---
title: Scratch
description: Scratch 二次开发纪要
published: true
date: 2020-05-13T14:03:33.905Z
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
> VideoStep.componentDidMount()
注释掉国外网站视频https://fast.wistia.com/assets/external/E-v1.js

4. locales/*.js
> 删除其他语言

5. src/lib/analytics.js
> 注销google跟踪分析代码

6. src/lib/libraries/*.json
> *.js 增加了分类
> *.json 增加了新的角色库内容

7. src/lib/project-fetcher-hoc.jsx
> 修改了assetHost， projectHost

8. src/lib/screen-utils.js
> 增强了对只能设备的支持， gui 宽度等于 min(设备宽度,当前gui 宽度)

9. src/lib/storage.js
> getAssetGetConfig() 修改了url         return `${this.assetHost}/assets/static/${asset.assetId}.${asset.dataFormat}`;

10. src/reducers/locales.js
> 修改为默认中文
```javascript
const initialState = {
    isRtl: false,
    locale: 'en',
    messagesByLocale: editorMessages,
    messages: editorMessages.en
};
```
## scratch-www