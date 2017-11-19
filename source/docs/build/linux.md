---
title:Linux环境下编译
---
# 获取源码并编译元界钱包

## 获取源码

元界核心代码托管在 <https://github.com/mvs-org/metaverse>
```bash
git clone https://github.com/mvs-org/metaverse.git
```

## 编译工具安装（如果已经装配请略过）

* C++编译器：要求支持C++14标准，通常是g++ 5/LLVM 8.0.0/MSVC14
* CMake 2.8+

## 元界核心钱包所依赖的库

元界所依赖的库编译依赖GNU toolchain\(automake/autoconf/libtool\), 请执行安装

```bash
yum/apt-get/brew install automake/autoconf/libtool
```

或者自行编译安装，版本不限定；


* boost 1.56 +
```bash
sudo yum/apt-get/brew install libboost-all-dev
```

* ZeroMQ 4.21 +
```bash
wget https://github.com/zeromq/libzmq/releases/download/v4.2.1/zeromq-4.2.1.tar.gz
cd zeromq-4.2.1
./autogen.sh
./configure
make -j4
sudo make install && sudo ldconfig
```

* spec256k1
```bash
git clone https://github.com/mvs-live/secp256k1
cd secp256k1
./autogen.sh
./configure --enable-module-recovery
make -j4
sudo make install && sudo ldconfig
```
