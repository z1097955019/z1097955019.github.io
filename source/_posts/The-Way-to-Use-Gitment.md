---
title: The_Way_to_Use_Gitment
date: 2017-12-29 23:40:51
categories: 
 - Study
 - Summery
 - programme
tags: Technology Text
---
# Gitment 的配置
1. GitHub授权接入

Gitment是使用的GitHub Issues作为评论系统，在接入Gitment前，需要获得GitHub的授权，获得相应的客户端id和客户端私钥，以备站点使用。具体步骤如下图所示：
![](The-Way-to-Use-Gitment/1.png)
![](The-Way-to-Use-Gitment/2.png)
2. next主题集成代码的修改
```
gitment:
  enable: true
  mint: true # RECOMMEND, A mint on Gitment, to support count, language and proxy_gateway
  count: true # Show comments count in post meta area
  lazy: false # Comments lazy loading with a button
  cleanly: false # Hide 'Powered by ...' on footer, and more
  language: zh-Hans
  github_user: #github的**用户名**
  github_repo: #随便找一个**公开**的仓库
  client_id: 
  client_secret: 
  proxy_gateway: # Address of api proxy, See: https://github.com/aimingoo/intersect
  redirect_protocol: # Protocol of redirect_uri with force_redirect_protocol when mint enabled
```
# 坑
* 请注意上述强调的字体