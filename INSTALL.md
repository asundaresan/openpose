# Installation 

## Clone openpose.git 

```
git clone https://github.com/asundaresan/openpose.git
```

## Install Dependencies

```
sudo apt-get install -y libgflags-dev libceres-dev libgoogle-glog-dev libleveldb-dev libhdf5-dev liblmdb-dev libprotobuf-dev libopencv-dev python-opencv libeigen3-dev libtinyxml-dev libtinyxml2-dev libvmmlib-dev libzmq-dev libatlas-dev libatlas-base-dev libboost1.58-all-dev libprotoc-dev protobuf-compiler libsnappy-dev keychain cmake libatlas-dev libatlas-base-dev
```

## Install nVidia drivers

Install nVidia driver, e.g. 384.111.

## Install CUDA

Works with version 8.

```
sudo apt-get install cuda
```

## Install cuDNN

Requires cudnn5.

```
sudo dpkg -i libcudnn5_5.1.5-1+cuda8.0_amd64.deb  libcudnn5-dev_5.1.5-1+cuda8.0_amd64.deb
```

## Build and install openpose

```
mkdir build 
cd build
cmake -DCMAKE_INSTALL_PREFIX=/opt/openpose ..
make 
sudo make install
```

