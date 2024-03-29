# Build SymuCore - SymuVia

![](https://img.shields.io/badge/platform-osx--64-blue) ![](https://img.shields.io/badge/platform-linux-green)

A simple project structure to Build `SymuVia`. 

1. Get the repo 
  `git clone https://github.com/becarie/symudev.git && cd build-symuvia`
2. Create the directory to build e.g `mkdir build`
3. Go to the coresonding directory `cd build` 
4. Generate config pointing to the place where the file `CMakeLists.txt` is placed `cmake ..`
5. Build your target via `cmake -build .` or `make`

## Dependencies 

On Linux `install` 

```
      apt-get update && apt-get install -y \
      wget bzip2 ca-certificates \
      xz-utils \
      build-essential \ 
      curl \   
      git \
      libxqilla-dev \
      libboost-all-dev \
      aptitude \
      gdal-bin \
      rapidjson-dev \
      libgdal-dev \
      unixodbc \
      libpq-dev &&\
      aptitude search -y \
      boost \
      && rm -rf /var/lib/apt/lists/*
```

On OS X `install`

```
      brew install boost boost-python3 gdal xqilla rapidjson unixodbc # python (optional) in case anaconda is not installed 
```
