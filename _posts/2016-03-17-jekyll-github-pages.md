---
layout: post
title: "jekyll github pages"
description: ""
category: 
tags: []
---
{% include JB/setup %}

## 创建自己的Github pages 

    登录github,New repository

## 安装Jekyll

安装环境为Win10 64位

## 下载Bootstrap模板

    $git clone https://github.com/plusjade/jekyll-boostrap.git jekyll

## 发布到Github

- git remote set-url origin https://github.com/lyon-neu.io/ `name`.git
- git add .
- git commit -m ''
- git push origin master
- git checkout -b gh-pages  
- 修改根目录下地_config.yml文件 
    production_url : http://lyon-neu.github.io
    JB：
        BASE_PATH : /jekyll-demo

查看bootstrap模板下的/asset/themes/目录，可以看到有bootstrap-3和twitter两个文件夹，实际布署的时候会提示找不到bootstrap/，所次将bootstrap-3里的文件全部复制到/themes/目录下

你可以直接 [下载 PDF]({{ site.url }}/assets/IADIS_submission_Lisa_W.pdf).