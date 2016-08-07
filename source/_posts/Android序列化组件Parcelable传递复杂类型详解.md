---
title: Android序列化组件Parcelable传递复杂类型详解.md
date: 2016-08-04 19:27:47
updated: 2016-08-04 19:27:47
tags:
- Android_SDK
- Parcelable
categories:
- Android
---

Android中实现序列化有两个选择：一是实现Serializable接口（是JavaSE本身就支持的），一是实现Parcelable接口（是Android特有功能，效率比实现Serializable接口高效，可用于Intent数据传递，也可以用于进程间通信（IPC））。实现Serializable接口非常简单，声明一下就可以了，而实现Parcelable接口稍微复杂一些，但效率更高，推荐用这种方法提高性能。
关于Parcelable基础网上已经有很多介绍，在这里就不多做赘述，可以参看一下文章：
[基本用法][1]
[与Serializable效率对比，某些情况下可达10倍][2]

## 复杂类型的传递
#### 传递Bitmap


  [1]: http://www.cnblogs.com/renqingping/archive/2012/10/25/Parcelable.html
  [2]: http://greenrobot.me/devpost/android-parcelable-serializable/

