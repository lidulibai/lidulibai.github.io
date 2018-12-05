---
title: docker_publish
date: 2018-12-05
tags:
---

docker save image image | gzip > publish.tar.gz

docker load < publish.tar.gz
