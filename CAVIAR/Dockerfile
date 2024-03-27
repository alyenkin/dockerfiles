FROM ubuntu:20.04

RUN apt-get update && apt-get install -yq --no-install-recommends \
  libblas-dev \
  liblapack-dev \
  wget \
  unzip \
  build-essential \
  libgsl-dev

RUN cd opt \
  && wget --no-check-certificate https://github.com/fhormoz/caviar/archive/master.zip \
  && unzip master.zip \
  && mv caviar-master caviar \
  && cd caviar/CAVIAR-C++ \
  && make
