FROM rocker/tidyverse:latest
USER root
LABEL maintainer="Akira Hasegawa <akira.hasegawa@riken.jp>"
ENV TZ JST-9
RUN apt-get update \
&& apt-get -y install \
vim \
less \
&& apt-get autoremove -y \
&& apt-get clean \
&& rm -rf /usr/local/src/*
RUN R -e "install.packages('Seurat',dependencies=TRUE, repos='http://cran.rstudio.com/')"
RUN R -e "install.packages('dplyr',dependencies=TRUE, repos='http://cran.rstudio.com/')"
RUN R -e "install.packages('Matrix',dependencies=TRUE, repos='http://cran.rstudio.com/')" 
RUN R -e "install.packages('umap',dependencies=TRUE, repos='http://cran.rstudio.com/')" 