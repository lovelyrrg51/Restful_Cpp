# Introduction
`Simple RestFul App with Cpp using crowcpp & cpp_redis`

# How to use
## 1. Environment
Make sure that install [redis-cli](https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-redis-on-ubuntu-22-04) and [cmake](https://orcacore.com/install-use-cmake-ubuntu-22-04/) on ubuntu.

## 2. Crowcpp & Cpp_Redis
### 2.1 How to download & install Crowcpp
From [Crowcpp](https://crowcpp.org/master/getting_started/setup/linux/), you could download `Crowcpp` to `./dependencies` directory and get how to install it.
### 2.2 How to download & cpp_redis
From [Cpp_Redis](https://github.com/cpp-redis/cpp_redis), you could download `Cpp_Redis` to `./dependencies` directory and get how to install it.

## 3. Build & Run
```
mkdir build && cd build
cmake ..
make
./cppREST
```
