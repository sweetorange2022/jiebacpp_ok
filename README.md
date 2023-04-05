# CppJieba [English](README_EN.md)

[![CMake](https://github.com/yanyiwu/cppjieba/actions/workflows/cmake.yml/badge.svg)](https://github.com/yanyiwu/cppjieba/actions/workflows/cmake.yml)
[![Author](https://img.shields.io/badge/author-@yanyiwu-blue.svg?style=flat)](http://yanyiwu.com/) 
[![Platform](https://img.shields.io/badge/platform-Linux,%20OS%20X,%20Windows-green.svg?style=flat)](https://github.com/yanyiwu/cppjieba)
[![Performance](https://img.shields.io/badge/performance-excellent-brightgreen.svg?style=flat)](http://yanyiwu.com/work/2015/06/14/jieba-series-performance-test.html) 
[![Tag](https://img.shields.io/github/v/tag/yanyiwu/cppjieba.svg)](https://github.com/yanyiwu/cppjieba/releases)
[![License](https://img.shields.io/badge/license-MIT-yellow.svg?style=flat)](http://yanyiwu.mit-license.org)
[![Build status](https://ci.appveyor.com/api/projects/status/wl30fjnm2rhft6ta/branch/master?svg=true)](https://ci.appveyor.com/project/yanyiwu/cppjieba/branch/master)

## 简介

CppJieba是"结巴(Jieba)"中文分词的C++版本,非常好用

<b>但是原作者将 limonp 库和本项目分开了，直接下载编译原作者的项目编译根本无法通过，可以直接下载本项目编译使用！不必再自己手动添加 limonp 库</b>

## 特性

+ 源代码都写进头文件`include/cppjieba/*.hpp`里，`include`即可使用。
+ 支持`utf8`编码。
+ 项目自带较为完善的单元测试，核心功能中文分词(utf8)的稳定性接受过线上环境检验。
+ 支持载自定义用户词典，多路径时支持分隔符'|'或者';'分隔。
+ 支持 `Linux` , `Mac OSX`, `Windows` 操作系统。

## 用法

### 依赖软件

* `g++ (version >= 4.1 is recommended) or clang++`;
* `cmake (version >= 2.6 is recommended)`;

### 下载和编译

```sh
git clone https://github.com/yanyiwu/cppjieba.git
cd cppjieba
mkdir build
cd build
cmake ..
make　-j4;
```

有兴趣的可以跑跑测试(可选):

```
make test
```

## Demo

```
./demo
```

结果示例：

```
我今天真的很开心
[demo] Cut With HMM
我/今天/真的/很/开心
```

  
  我觉得对于一般场景来说HMM就够用了，比较符合我们的说话停顿、分割习惯。　　
  
  欢迎start和关注！
