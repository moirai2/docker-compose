# docker-compose
Studying docker-compose examples

## Requirements
* Docker
* docker-compose

### Examples

#### flask-redis

* Based on: https://www.python.ambitious-engineer.com/archives/1630
* Example using
  * flask - https://flask.palletsprojects.com/en/2.0.x/
  * redis - https://redis.io
* Access http://localhost:5000 of your computer to see.
```
cd flask-redis/
docker-compose build
docker-compose up -d
```
* To end the server.
```
docker-compose down
```

#### flask-mysql

* Based on: https://qiita.com/kai_kou/items/5d73de21818d1d582f00#flask-restful
* Example using
  * MySQL - https://www.mysql.com/jp/
  * Flask - https://flask.palletsprojects.com/en/2.0.x/
  * Flask-RESTful
  * SQLAlchemy
  * Flask-SQLAlchemy
  * Flask-Migrate
  * Flask-Marshmallow
  * marshmallow-sqlalchemy
  * PyMySQL
  * Gunicorn

* To check if mysql service is up...
```
docker-compose build db
docker-compose up -d db
docker-compose exec db mysql -u root -p
show databases;
exit
docker-compose down
```

#### jupyterlab

* docker environment for hosting jupyterlab servers
  * jupyterlab - environment for running common python
  * jupyterlab-cellrank - environment for running velocyto, scvelo, scanpy
  * jupyterlab-rstudio - environment for running Rstudio
  * jupyternotebook - environment for running older version of jupyterlab

#### nginx-php-mysql

* docker environment for combining nginx, php and mysql
