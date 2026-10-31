## 浏览器选择

<img src="https://github.com/n7n8/ah-browser-fragmentation/blob/main/Media/EdgeBrowser.avif" width="100" />

推荐使用Microsoft Edge，在中国大陆各大应用商店、[Google Play](https://play.google.com/store/apps/details?id=com.microsoft.emmx)均可下载

## 系统Webview更新

<p align="left">
   <img src="https://github.com/n7n8/ah-browser-fragmentation/blob/main/Media/Android%20System%20WebView.png" width="50" alt="Logo">
   <img src="https://github.com/n7n8/ah-browser-fragmentation/blob/main/Media/HuaweiWebview.png" width="50" alt="Logo">
</p>
<p align="left"><sup>
   Google Webview | Huawei Webview
</sup></p>

以下建议有一定动手能力的用户采用。

### 如何确定你的手机是哪种 Webview？

1. 打开“开发者选项”，点击“WebView 实现”。如果发现有“Android System Webview”选项，说明其支持Google Webview；如果只有“Huawei Webview”，说明其只支持Huawei Webview；如果只有“Hihonor Webview”，我的教程也救不了你😅

2. 安装[LibChecker](https://github.com/LibChecker/LibChecker)，确保打开“显示系统应用”，搜索“Webview”。在搜索到的app中对照app包名：
- com.google.android.webview→Google Webview
- com.huawei.webview→Huawei Webview
- com.amazon.webview→Amazon Webview
- com.android.webview→AOSP Webview
- com.hihonor.webview→Honor Webview

### Google Webview

优先级：Google Play → apk直接安装 → 小米特殊处理

1. [Google Play](https://play.google.com/store/apps/details/Android+System+WebView?id=com.google.android.webview)

2. apk直接安装

> 请用以下链接获取新版Google Webview的apk安装包↓
>
> [APKMirror](https://www.apkmirror.com/apk/google-inc/android-system-webview) [Uptodown](https://android-system-webview.en.uptodown.com/android) [APKPure](https://apkpure.com/android-system-webview-app/com.google.android.webview/amp)
> 
> （中国大陆网络条件）[apkz](https://www.apkz.com/app/com.google.android.webview/en.html) [当快软件园](https://www.downkuai.com/android/167450.html)
> 
> <!-- 注意：请不要用APKPure下载非系统应用，尤其是Telegram -->
> 
> 对于（支持Google Webview的）vivo、OPPO、荣耀、三星、联想、中兴 手机用户，直接安装下载好的Android System Webview apk即可

3. 小米特殊处理

> 如果你是小米手机用户，不能直接安装系统apk，且不方便使用Google Play，建议使用PC adb安装或Shizuku+InstallerX Revived的组合
> 
> 注意：需要确保开启开发者选项、adb调试、USB安装
>
> adb安装命令：
> 
> ```
> adb install <APK文件路径>
> ```
> 
> >
> > 如果使用Shizuku+InstallerX Revived的组合：
> >
> > [Shizuku下载链接（rushiranpise/Shizuku-Next）](https://github.com/rushiranpise/Shizuku-Next) [Shizuku教程](https://shizuku.rikka.app/zh-hans/guide/setup)
> >
> > InstallerX Revived下载链接：
[GitHub](https://github.com/wxxsfxyzm/InstallerX-Revived) [Telegram](https://t.me/installerx_revived)
> >
> > 对于小米手机用户，InstallerX Revived的Shizuku权限设置好后，建议在文件管理app中，长按apk文件，点击“分享-InstallerX Revived”进行安装

### Huawei Webview

132版本的[Huawei Webview](https://github.com/n7n8/ah-browser-fragmentation/releases/tag/132.0.6.304)
[（TG Channel）](https://t.me/kkdx10)

### Amazon Webview

[APKMirror下载链接](https://www.apkmirror.com/apk/amazon-mobile-llc/amazon-system-webview/)
