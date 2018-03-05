---
title: 'GCE,AWS,site5主机小对比'
id: 56
categories:
  - linux
date: 2015-06-03 23:08:32
tags:
---

最近分别用了这三家的主机，因为是博客，对于运行速度和软件生态没有要求．

主要是价格和连接速度的比较：

#### 价格

*   AWS 新用户可以免费用micro用一年，还有RDS数据库也可以用一年．不过后面费用就有点贵了，日本机房 t2.small 1CPU, 2GB $21.90/月
*   GCE  (google Compute Engine) 可以免费三个月,之后 1CPU,1.7GB $17/月
*   site5 没有任何优惠活动，2CPU,1GB $27.5/月

#### 速度

*   AWS 日本，大陆ping在150-300之间，速度一般
*   GCE 台湾，大陆ping50-100左右．没有遇到过"超时"的情况
*   site5 香港，用的好像是IBM softlayer的机房，ping 30左右，广东地区可以到10+，非常流畅，适合搭代理
*   IBM softlayer在香港的机房一直很想买，无奈起步价太贵了

### 软件

*   AWS 毫无疑问很丰富，但对于博客来说大炮打蚊子
*   GCE 也没什么问题，唯一一个就是发不了邮件，google自己封锁了邮件发送端口，能收但不能往外发，只能专门购买其它家的邮件服务
*   site5 基本没什么管理功能，缺少镜像快照支持，升级机器也很不方便
*   以上这三家都支持Centos7.0 64bit
综合各方面，最后决定继续使用google的服务

PS. 之前是想用腾讯云香港机房的，不过香港机房也要求备案了，好麻烦算了