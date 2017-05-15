---
title: vim为主提供eclipse部分特性的使用eclim
date: 2017-05-14 14:17:38
tags:
---
## 启动eclim服务
执行$ECLIPSE_HOME/eclimd或者%ECLIPSE_HOME%\eclimd.bat

## 关闭eclim服务
在VIM执行
> :ShutdownEclim

## maven创建项目
    mvn archetype:generate

## 把maven项目转换成eclipse项目
    cd <project_dir>
    mvn eclipse:eclipse

## 导入项目到eclipse或者说让eclim跟踪这个项目
VIM编辑项目根目录 > vim <project_dir>
:MvnRepo
:ProjectImport /path/to/new/project
