# 移动端浏览器碎片化记录（排除iOS）
> [!NOTE]
> 一个主要平台如果有能顺利运行Web的主流性能区间与主流系统版本，这个平台就必须要有统一的Web内核治理。

### 关于本记录

国际统计机构（如StatCounter）对中国大陆Android浏览器市场的统计存在明显偏差，经常[显示Chrome占据多数份额](https://gs.statcounter.com/browser-market-share/mobile/china)，这与中国大陆用户的实际情况完全不符。

更重要的是，这些统计几乎完全不关注浏览器内核版本的碎片化问题。本仓库聚焦Android&HarmonyOS生态，记录各OEM浏览器、中国大陆第三方浏览器、国际第三方浏览器、常用app内嵌内核的实际Chromium/Firefox版本情况。

<p align="center">
   <img src="./Media/SamsungBrowser.png" width="50" alt="Logo">
   <img src="./Media/VivoBrowser-System-Round.png" width="50" alt="Logo">
   <img src="./Media/OPPOBrowser.png" width="50" alt="Logo">
   <img src="./Media/XiaomiBrowser.png" width="50" alt="Logo">
   <img src="./Media/HonorBrowser.png" width="50" alt="Logo">
</p>
<p align="center"><sup>
   Android • 主要的OEM浏览器图标（除了Chrome）
</sup></p>

### 📂 目录结构与设计说明
```ah-browser-fragmentation
tree/main/
├── 2026/
├── Media/
├── Archive/
├── Posts/
└── TL;DR/
```

*   **`2026/`**：
    *   包含这一年的浏览器内核版本数据。
*   **`Media/`**：
    *   用于存储图片内容。
*   **`Archive/`**：
    *   存档及备份[“特别感谢”](https://github.com/n7n8/ah-browser-fragmentation/blob/main/README.md#%E7%89%B9%E5%88%AB%E6%84%9F%E8%B0%A2%E4%BB%A5%E4%B8%8B%E7%BD%91%E9%A1%B5%E5%B7%B2%E5%A4%87%E4%BB%BD%E8%87%B3archive%E6%96%87%E4%BB%B6%E5%A4%B9)中的内容。
*   **`Posts/`**：
    *   主要讲述中国大陆Android浏览器内核的更新机制。
*   **`TL;DR/`**：
    *   我懒得概括了。😅

### 目前中国大陆Android的浏览器兼容性基线（仅供参考）

1、Chromium 97（正在过时）

- [x] 百度app（淘汰时间：2026年9月；可更新）
- [x] 荣耀套壳浏览器（淘汰时间：2026年1月；对旧荣耀手机来说近乎“没有更新能力”，不是不能装com.honor.browser，而是大多数用户不会专门装额外的浏览器）

2、Chromium 114

- [x] 鸿蒙4 华为浏览器（淘汰时间：2026年3月畅享90系列发布；实际几乎不可更新）
- [x] 鸿蒙4 Huawei Webview（淘汰时间：2026年3月畅享90系列发布；理论上有132版本Huawei Webview，实际几乎不可更新）
- [ ] OPPO浏览器（Chromium 115）（未淘汰；可更新）
- [x] 荣耀浏览器（Chromium 116）（淘汰时间：2026年10月；可更新）
- [ ] Hihonor Webview（Chromium 116）（未淘汰，仍在新的荣耀低端机型存在；没有更新能力）

### 特别感谢（以下网页已备份至[/Archive](https://github.com/n7n8/ah-browser-fragmentation/tree/main/Archive)文件夹）
1. [🗂 前端版本兼容问题的探索 - 卤代烃实验室](https://supercodepower.com/fontend-target/)
2. [💖【投票+测评】你平时用的浏览器内核版本 - 夜雨聆风](https://www.yeyulingfeng.com/83723.html)
3. [关于手机webview内核、默认浏览器、各家小程序的渲染层浏览器的区别和兼容性 - DCloud社区](https://ask.dcloud.net.cn/m/article/1318)
4. [2021年国产Chrome套壳浏览器的版本号 - zhihu - liu-zhi-qiang-36-54](https://zhuanlan.zhihu.com/p/405207457)
5. [【安全报告】2017年第一季度 安卓系统安全性生态环境研究 - 安全KER](https://www.anquanke.com/post/id/86161)

### 公开数据来源（但不是本项目数据唯一来源）
1. [Chromium Dash - Schedule](https://chromiumdash.appspot.com/schedule)
2. [Microsoft Edge release notes for Stable Channel | Microsoft Learn](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-relnote-stable-channel)
3. [Firefox Release Calendar](https://whattrainisitnow.com/calendar/)
4. [ArkWeb简介-指南与API参考-指南-应用框架-ArkWeb（方舟Web）-ArkWeb简介 - 华为HarmonyOS开发者](https://developer.huawei.com/consumer/cn/doc/doccenter-capabilities/web-component-overview)
5. [小程序交流专区 | 微信开放社区](https://developers.weixin.qq.com/community/develop/mixflow)
6. [关于腾讯浏览服务-官网文档中心 - 腾讯浏览服务](https://x5.tencent.com/docs.html#AboutTBS)
