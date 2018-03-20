# Installation 

## Clone openpose.git 

```
git clone https://github.com/asundaresan/openpose.git
```

## Install Dependencies

```
sudo apt-get install -y libgflags-dev libceres-dev libgoogle-glog-dev libleveldb-dev libhdf5-dev liblmdb-dev libprotobuf-dev libopencv-dev python-opencv libeigen3-dev libtinyxml-dev libtinyxml2-dev libvmmlib-dev libzmq-dev libatlas-dev libatlas-base-dev libboost1.58-all-dev libprotoc-dev protobuf-compiler libsnappy-dev keychain
```

## Install nVidia drivers

Install nVidia driver, e.g. 384.111.

## Install CUDA

```
sudo apt-get install cuda
```

## Install cuDNN

```
sudo dpkg -i libcudnn7_7.0.5.15-1+cuda9.1_amd64.deb  libcudnn7-dev_7.0.5.15-1+cuda9.1_amd64.deb
```

## Build and install openpose

```
mkdir build 
cd build
cmake -DCMAKE_INSTALL_PREFIX=/opt/openpose ..
make 
sudo make install
```

