---
title: hexo配置无密码发布到github
date: 2017-05-14 10:02:17
tags:
---
## 先配置hexo的配置文件_config.yml
    deploy:
        type: git
        repository: git@github.com:yourname/yourname.github.io.git
        branch: master

## 生成SSH key
    ssh-keygen -t rsa -C "yourname@youremail.com"

## 配置github,添加你这台机器的key
复制.ssh目录下id_rsa.pub的所有内容，然后在github的Settings里面添加SSH key,
titile随便写，建议为自己能辨识所哪台电脑，内容就粘贴上刚刚复制的内容。

## 配置git全局变量
    git config --global user.name "yourname"
    git config --global user.email "your_email@youremail.com"

## 测试连接
    ssh -T git@github.com

## 成果
到此使用命令> hexo d 已经不许要输入命令就可以部署了
