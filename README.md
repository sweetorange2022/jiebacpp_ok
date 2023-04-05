# jiebacpp_ok
补充了原作者缺少的limonp库，使得cppjieba可直接编译使用  
# CppJieba


## 简介

CppJieba是"结巴(Jieba)"中文分词的C++版本，在中文分词方面非好用！


<b>
但是原作者将CppJieba和limonp库分开了，直接下载源代码编译无法通过，需要加入limonp库，这个版本是已经加入limonp库的，可直接参照下面的用法使用！
</b>

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
git clone https://github.com/sweetorange2022/jiebacpp_ok.git
cd cppjieba/build
make clean
cmake ..
make
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


## 线上演示

[Web-Demo](http://cppjieba-webdemo.herokuapp.com/)
(建议使用chrome打开)



