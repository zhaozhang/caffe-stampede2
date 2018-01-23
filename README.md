# caffe-maverick
libraries and makefiles for caffe deployment on Maverick

Makefile.config -- for Caffe
Makefile -- for MXNet
config.mk -- for MXNet

# caffe
## boost

* ./bootstrap.sh --prefix=/home1/00946/zzhang/caffe/boost
* ./b2 --prefix=/home1/00946/zzhang/caffe/boost 

## hdf5

*  ./configure --prefix=/home1/00946/zzhang/caffe/hdf5
* make
* make install

## lmdb

*  make
*  cp *.h ../../../include
*  cp *.so ../../../lib

## protocol-buffer

*   ./configure --prefix=/home1/00946/zzhang/caffe/protocol-buffer
*  make
*  make install

## glog

*  ./configure --prefix=/home1/00946/zzhang/caffe/glog
*  make
*  make install

## snappy

*  ./configure --prefix=/home1/00946/zzhang/caffe/snappy
*  make
* make install

## leveldb

*  make
*  mv out-shared ../lib
*  cp -r include ../

## opencv

*  cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/home1/00946/zzhang/caffe/opencv ..
*  make
*  make install

