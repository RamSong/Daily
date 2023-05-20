---
title: Cloudflare部署Hexo糟心历程
date: 2023-05-20 19:36:59
tags:
---

#起
Vercel部署不能自定义SSL
众所周知 Let's Encrypt 证书 OCSP 被污染了
虽然影响不是很大但心里就是不爽
听说 Cloudflare Pages 也不错
开整！

#升
原来想着本地渲染推送到 Github
再同步到 Cloudflare Pages
考虑到自动部署
就打算把整个后端都上传
用 Cloudflare 服务器渲染界面

#落
我这辈子都没这么无语过
![OOe0bP.png](https://i.imgtg.com/2023/05/20/OOe0bP.png)
花了一个小时才搞定
Cloudflare 对 Hexo 的支持也太差了

#总
总结下遇到的几个问题
1. 主题当做子模块
 导致