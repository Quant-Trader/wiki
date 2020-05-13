---
title: Scratch
description: Scratch 二次开发纪要
published: true
date: 2020-05-13T13:37:31.008Z
tags: 
---

# SCARTCH
## scratch-gui
1. src/containers/library-item.jsx
> render()
修改了iconURl的默认网址

2. src/containers/gui.jsx
> 目的： 将VM接口暴露到外部js文件， 可以通过vm 发送键盘消息
componentDidMount()
增加了
componentDidUpdate()

3. src/components/cards/cards.jsx
》 VideoStep.componentDidMount()
注释掉国外网站视频https://fast.wistia.com/assets/external/E-v1.js