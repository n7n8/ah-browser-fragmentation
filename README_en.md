# Mobile Browser Fragmentation Record (Excluding iOS)

> [!NOTE]
> If a major platform has a mainstream performance range and mainstream system versions capable of running the Web smoothly, this platform must have unified Web kernel governance.

[中文](./README.md)

### [How to Update the Browser Kernel on Android (Mainland China)](./Posts/%E4%B8%AD%E5%9B%BD%E5%A4%A7%E9%99%86Android%E7%94%A8%E6%88%B7%E5%A6%82%E4%BD%95%E6%9B%B4%E6%96%B0%E6%B5%8F%E8%A7%88%E5%99%A8%E5%86%85%E6%A0%B8.md)

### About This Record
International statistics agencies (such as StatCounter) have obvious deviations in their statistics of the Android browser market in mainland China, often [showing Chrome occupying the majority share](https://gs.statcounter.com/browser-market-share/mobile/china), which is completely inconsistent with the actual situation of mainland Chinese users.
More importantly, these statistics almost completely ignore the fragmentation of browser kernel versions. This repository focuses on the Android & HarmonyOS ecosystem, recording the actual Chromium/Firefox versions of various OEM browsers, third-party browsers in mainland China, international third-party browsers, and embedded kernels in commonly used apps.

<p align="center">
   <img src="./Media/SamsungBrowser.png" width="50" alt="Samsung">
   <img src="./Media/LenovoBrowser.png" width="50" alt="Lenovo">
   <img src="./Media/VivoBrowser-System-Round.png" width="50" alt="vivo">
   <br>
   <img src="./Media/OPPOBrowser.png" width="50" alt="OPPO">
   <img src="./Media/XiaomiBrowser.png" width="50" alt="Xiaomi">
   <img src="./Media/HonorBrowser.png" width="50" alt="HONOR">
</p>
<p align="center"><sup>
   Android • Major OEM browser icons (except <a href="https://play.google.com/store/apps/details?id=com.android.chrome">Chrome</a>)
</sup></p>

### 📂 Directory Structure and Design Notes
```ah-browser-fragmentation
tree/main/
├── 2026/
├── Media/
├── Archive/
├── Posts/
└── TL;DR/
```
*   **`2026/`**:
    *   Contains browser kernel version data for this year.
*   **[Media/](./Media/)**:
    *   Used to store image content.
*   **[Archive/](./Archive/)**:
    *   Archive and backup of the content in ["Special Thanks"](./README_en.md#special-thanks-the-following-webpages-have-been-backed-up-to-the-archive-folder).
*   **[Posts/](./Posts/)**:
    *   Mainly describes the update mechanism of Android browser kernels in mainland China.
*   **[TL;DR/](./TL;DR/)**:
    *   I'm too lazy to summarize. 😅

### Current Browser Compatibility Baseline for Android in Mainland China (For Reference Only)
Note: "Phased out" refers to at least one of the following: "kernel version has been replaced by a higher version", "new pre-installation has been stopped", "software has been removed from shelves/distribution stopped".
1. Chromium 97 (becoming obsolete)
- [x] Baidu App (phased out: September 2026; updatable)
- [x] Honor shell browser (phased out: January 2026; for old Honor phones, it is almost "no update capability"—it's not that you cannot install com.honor.browser, but most users won't specifically install an additional browser)
2. Chromium 114
- [x] HarmonyOS 4 Huawei Browser (phased out: March 2026, Enjoy 90 series release; actually almost unupdatable)
- [x] HarmonyOS 4 Huawei Webview (phased out: March 2026, Enjoy 90 series release; theoretically there is version 132 Huawei Webview, but actually almost unupdatable)
- [ ] OPPO Browser (Chromium 115) (not phased out; updatable)
- [x] Honor Browser (Chromium 116) (phased out: October 2026; updatable)
- [ ] Hihonor Webview (Chromium 116) (not phased out, still exists on new Honor low-end models; no update capability)

### Special Thanks (The following webpages have been backed up to the [/Archive](./Archive) folder)
1. [🗂 Exploration of Frontend Version Compatibility Issues - Halohydrocarbon Laboratory](https://supercodepower.com/fontend-target/)
2. [💖【Vote + Review】What Browser Kernel Version Do You Usually Use - Night Rain Listening to Wind](https://www.yeyulingfeng.com/83723.html)
3. [About the Differences and Compatibility of Mobile WebView Kernels, Default Browsers, and Rendering Layer Browsers of Various Mini Programs - DCloud Community](https://ask.dcloud.net.cn/m/article/1318)
4. [2021 Version Numbers of Domestic Chrome Shell Browsers - liu-zhi-qiang-36-54 - Zhihu](https://zhuanlan.zhihu.com/p/405207457)
5. [【Security Report】Research on Android System Security Ecological Environment in Q1 2017 - Security KER](https://www.anquanke.com/post/id/86161)
6. [Complete Tutorial on WebView Update and Upgrade for Android TV Boxes - Bilibili](https://www.bilibili.com/opus/1141451214686257177)
7. [【Tinkering】Magic Box CM311-1A Tinkering Notes, Successfully Running "WebView TV", Smooth Live Streaming - Web TV - WeChat Official Account](https://mp.weixin.qq.com/s?__biz=MzkyNTg3NTIyNw==&mid=2247484014&idx=1&sn=8e876c72ca36c4e028405d9ccd7fa221)
8. [After Research, the Android Turnaround Theory Goes Bankrupt - Coolapk](https://www.coolapk.com/feed/67764470)
9. [Using Honor Phones, Say Goodbye to Lightweight Browsers #android webview #hihonor webview - Honor Club](https://club.honor.com/cn/thread-29317614-1-1.html)

### Recommended GitHub Repositories
1. [JonaNorman/WebViewUpgrade | Android WebView Kernel Upgrade Without Installation](https://github.com/JonaNorman/WebViewUpgrade)
2. [JonaNorman/WebViewPackage | Collecting and Archiving Android WebView APKs from Various Manufacturers](https://github.com/JonaNorman/WebViewPackage)
3. [zoulin3/force_system_webview | Force Android Apps to Use System WebView](https://github.com/zoulin3/force_system_webview)
4. [entr0pia/trichromelibrary-squoosh | Remove Outdated TrichromeLibrary](https://github.com/entr0pia/trichromelibrary-squoosh)
5. [dust-yu/sample_webview_android](https://github.com/dust-yu/sample_webview_android)
6. [daybreak1929/ViaBrowserCollection | Via Browser Collection](https://github.com/daybreak1929/ViaBrowserCollection)

### Recommended Gitee Repositories
1. [Half Dream Half Awake/Via Browser Collection](https://gitee.com/daybreak166/ViaBrowserCollection)

### Public Data Sources (But Not the Only Sources of This Project's Data)
1. [Chromium Dash - Schedule](https://chromiumdash.appspot.com/schedule)
2. [Microsoft Edge release notes for Stable Channel | Microsoft Learn](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-relnote-stable-channel)
3. [Firefox Release Calendar](https://whattrainisitnow.com/calendar/)
4. [Supported browsers | Baseline](https://web-platform-dx.github.io/supported-browsers/?target=widelyAvailable)
5. [ArkWeb Introduction - Guide and API Reference - Guide - Application Framework - ArkWeb (Ark Web) - ArkWeb Introduction - Huawei HarmonyOS Developer](https://developer.huawei.com/consumer/cn/doc/doccenter-capabilities/web-component-overview)
6. [Mini Program Exchange Zone | WeChat Open Community](https://developers.weixin.qq.com/community/develop/mixflow)
7. [About Tencent Browsing Service - Official Website Documentation Center - Tencent Browsing Service](https://x5.tencent.com/docs.html#AboutTBS)
8. [U4 Platform Status](https://developers.uc.cn/features/features.html)
