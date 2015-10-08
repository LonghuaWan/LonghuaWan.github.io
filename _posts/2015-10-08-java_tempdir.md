---
layout: post
tags: jvm参数 tmpdir
date: 2015-10-08 13:27
thumbnail: http://www.oracle.com/ocom/groups/public/@otn/documents/digitalasset/1612441.gif
title: Java tempdir
published: true
---
java.io.tmpdir is a standard Java system property which is used by the disk-based storage policies. It determines where the JVM writes temporary files, including those written by these storage policies (see Section 4 and Appendix A.6). The default value is typically "/tmp" on Unix-like platforms.
设置JAVA临时文件路径：
java -Djava.io.tmpdir=/temp
在ubuntu下默认是/tmp下
在JAVA程序中可以通过如下代码获取:
System.out.println(System.getProperty("java.io.tmpdir"));
可以通过如下语句在代码中设置：
System.setProperty("java.io.tmpdir", "/temporary");

[参考地址:]http://stackoverflow.com/questions/10108262/not-able-to-change-java-io-tmpdir
