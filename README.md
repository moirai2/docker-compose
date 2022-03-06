# docker-compose
Studying docker-compose examples

## Requirements
* Docker
* docker-compose

### Examples

#### flask-redis

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
