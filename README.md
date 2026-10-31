# 移动端浏览器碎片化记录（排除iOS）
> [!NOTE]
> 一个主要平台如果有能顺利运行Web的主流性能区间与主流系统版本，这个平台就必须要有统一的Web内核治理。

### [如果你想更新浏览器内核（仅限Android）](https://github.com/n7n8/ah-browser-fragmentation/blob/main/Posts/%E4%B8%AD%E5%9B%BD%E5%A4%A7%E9%99%86Android%E7%94%A8%E6%88%B7%E5%A6%82%E4%BD%95%E6%9B%B4%E6%96%B0%E6%B5%8F%E8%A7%88%E5%99%A8%E5%86%85%E6%A0%B8.md)

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
   Android • 主要的OEM浏览器图标（除了<a href="https://play.google.com/store/apps/details?id=com.android.chrome">Chrome</a>）
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
6. [安卓电视盒子WebView更新升级完整教程 - 哔哩哔哩](https://www.bilibili.com/opus/1141451214686257177)
7. [【折腾】魔百盒 CM311-1A 折腾记，成功运行“WebView 电视”，流畅看直播 - 网页电视 - 微信公众号](https://mp.weixin.qq.com/s?__biz=MzkyNTg3NTIyNw==&mid=2247484014&idx=1&sn=8e876c72ca36c4e028405d9ccd7fa221)
8. [经过研究，安卓翻身论破产 - 酷安](https://www.coolapk.com/feed/67764470)

### GitHub仓库推荐
1. [JonaNorman/WebViewUpgrade | Android免安装升级WebView内核](https://github.com/JonaNorman/WebViewUpgrade)
2. [JonaNorman/WebViewPackage | 收集和归档各厂商 Android WebView APK](https://github.com/JonaNorman/WebViewPackage)
3. [zoulin3/force_system_webview | 强制 Android 应用使用系统 WebView](https://github.com/zoulin3/force_system_webview)
4. [entr0pia/trichromelibrary-squoosh | 移除过时的 TrichromeLibrary](https://github.com/entr0pia/trichromelibrary-squoosh)
5. [dust-yu/sample_webview_android](https://github.com/dust-yu/sample_webview_android)
6. [daybreak1929/ViaBrowserCollection | Via浏览器收藏合集](https://github.com/daybreak1929/ViaBrowserCollection)

### Gitee仓库推荐
1. [半梦半醒/Via浏览器收藏合集](https://gitee.com/daybreak166/ViaBrowserCollection)

### 公开数据来源（但不是本项目数据唯一来源）
1. [Chromium Dash - Schedule](https://chromiumdash.appspot.com/schedule)
2. [Microsoft Edge release notes for Stable Channel | Microsoft Learn](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-relnote-stable-channel)
3. [Firefox Release Calendar](https://whattrainisitnow.com/calendar/)
4. [Supported browsers | Baseline](https://web-platform-dx.github.io/supported-browsers/?target=widelyAvailable)
5. [ArkWeb简介-指南与API参考-指南-应用框架-ArkWeb（方舟Web）-ArkWeb简介 - 华为HarmonyOS开发者](https://developer.huawei.com/consumer/cn/doc/doccenter-capabilities/web-component-overview)
6. [小程序交流专区 | 微信开放社区](https://developers.weixin.qq.com/community/develop/mixflow)
7. [关于腾讯浏览服务-官网文档中心 - 腾讯浏览服务](https://x5.tencent.com/docs.html#AboutTBS)
8. [U4 Platform Status](https://developers.uc.cn/features/features.html)
