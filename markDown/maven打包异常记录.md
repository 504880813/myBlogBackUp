---
title: maven打包编译异常解决
date: 2017年9月14日16:47:13
categories:
tags:
     - maven
---
  之前在本地自己创建项目然后自己打包 没有任何问题<br >
  后来相同的配置没有通过git，直通通过压缩包拷贝给同事之后,同事编译失败,一直报错<br >
  org.apache.maven.plugin.compiler.CompilationFailureException: Compilation failure<br >
  并且出来 javac 乱码 `<options> <source files>`<br >
  后来通过网上的一些方法 比如 修改setting.xml配置 和 pom配置，修改ieda编码，修改项目编码 都没有解决问题。<br >
  最后看到控制台 乱码 决定再尝试一下成功解决。<br >
  修改idea中的maven配置 将maven的runner的运行编码修改为GB2312后成功解决 如 下图

![](https://i.imgur.com/nTGqztC.png)
  
