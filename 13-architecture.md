---
layout: default
title: 架构设计
---

# 架构设计
{:.no_toc}

* 目录
{:toc}

## 架构问题
图片的访问速度

## 解决方案
**解决方案概要：** 使用七牛云作为图片和视频等资源的服务器。

**因素：**
- 从打开页面后图片加载的速度提升
- 多用户打开图片的速度提升

**解决方案：**
将原本在阿里云服务器上面的图片资源，迁移到七牛云的服务器上。使用七牛云的图片CDN服务，可以大大提升图片访问的速度和稳定性。在数据库中，只需要保存图片的特定的id，然后将id返回给前端。前端上传图片的时候，只需要直接上传到七牛云，然后把它的id发送给后端入库。

**动机**
目前七牛云的图片服务器在1G流量下是免费的，所以在经济上毫无压力。
同时对于我们服务的用户来说，打开图片的速度和用户的使用感受非常有关系，所以这样子的改变势在必行。

**未解决问题**
暂无

**其他可以选择的方案**
阿里云也有OSS服务器，不过使用起来没有那么方便。

**逻辑视图**
![](./assets/pics/ljst.png)

**物理视图**
![](./assets/pics/wlst.png)