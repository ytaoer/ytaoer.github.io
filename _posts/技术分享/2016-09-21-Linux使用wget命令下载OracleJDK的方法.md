---
layout: post
category : 技术分享
tagline:
tags : [编程]
excerpt :
title_cn: Linux使用wget命令下载OracleJDK的方法
description:  Oracle官网上需要点击accept licence的才能下载jdk，导致wget下载失败......
---
{% include JB/setup %}

## 说明

  Oracle官网上下载jdk，需要点击accept licence的才能下载，导致wget命令下载失败，使用下面的方法，直接可以下载

## 操作步骤

  用火狐浏览器打开Oracle官网的下载链接，我这里以jdk8 为例

>
>  http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
>
>
>  选择accept licence
>
>  选择需要下载的版本,点击下载
>
>  复制下载链接
>
>  http://download.oracle.com/otn-pub/java/jdk/8u101-b13/jdk-8u101-linux-x64.tar.gz?AuthParam=1474440873_207158c2eb5a557d3c268fda98cc5fef
> 
>  复制这个链接
>
>  wget  http://download.oracle.com/otn-pub/java/jdk/8u101-b13/jdk-8u101-linux-x64.tar.gz?AuthParam=1474440873_207158c2eb5a557d3c268fda98cc5fef 
>

## 注意

  此方法获取到的链接有一定的时效性，需要每次下载都复制一次下载链接
  
  也可按F12 查看“网络”请求来确定下载链接