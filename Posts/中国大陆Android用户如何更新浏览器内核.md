## 浏览器选择

<img src="../Media/EdgeBrowser.avif" alt="Microsoft Edge" width="100">

推荐使用Microsoft Edge，在中国大陆各大应用商店、[Google Play](https://play.google.com/store/apps/details?id=com.microsoft.emmx)均可下载

## 系统Webview更新

<p align="left">
   <img src="../Media/Android%20System%20WebView.png" width="50" alt="Android System Webview">
   <img src="../Media/HuaweiWebview.png" width="50" alt="Huawei Webview">
</p>
<p align="left"><sup>
   Google Webview | Huawei Webview
</sup></p>

以下建议有一定动手能力的用户采用。

### 如何确定你的手机是哪种 Webview？

配置开发者选项教程：[全球站](https://developer.android.com/studio/debug/dev-options?hl=zh-cn) [CN站](https://developer.android.google.cn/studio/debug/dev-options?hl=zh-cn)

1. 打开“开发者选项”，点击“WebView 实现”。如果列表中有“Android System Webview”选项，说明其支持Google Webview；华为（非鸿蒙5+）手机可能只有“Huawei Webview”；如果只有“Hihonor Webview”，我的教程也救不了你😅

2. 安装[LibChecker](https://github.com/LibChecker/LibChecker)，确保打开“显示系统应用”，搜索“Webview”。在搜索到的app中对照app包名：

- `com.google.android.webview`→Google Webview
- `com.huawei.webview`→Huawei Webview
- `com.amazon.webview`→Amazon Webview
- `com.android.webview`→AOSP Webview
- `com.hihonor.webview`→Hihonor Webview

### Google Webview（Android 10+）

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
> 对于（支持Google Webview的）vivo（含 iQOO）、OPPO（含 一加、Realme）、荣耀、三星、联想（含 摩托罗拉）、中兴（含 红魔、努比亚）手机用户，直接安装下载好的Android System Webview apk即可

3. 小米特殊处理

> 如果你是 **不方便使用Google Play** 的小米手机用户，建议使用 PC adb 安装或 Shizuku + InstallerX Revived 的组合（因为不能直接安装系统 apk）
> 
> 注意：需要确保开启开发者选项、USB调试、USB调试（安全设置）、USB安装
> 
> ① PC adb 安装
>
> （adb 包含在 Android SDK Platform-Tools 软件包中）
>
> Android SDK Platform-Tools下载链接：
>
> [全球站](https://developer.android.com/tools/releases/platform-tools#downloads) [CN站](https://developer.android.google.cn/tools/releases/platform-tools#downloads)
>
> adb安装命令：
> 
> ```
> adb install <APK文件路径>
> ```
> ---
> ② Shizuku + InstallerX Revived 组合
> 
> <img src="https://github.com/rushiranpise/Shizuku-Next/blob/master/docs/logo.png" alt="Shizuku-Next" width="16" /> Shizuku（rushiranpise/Shizuku-Next）：
> 
> [GitHub下载链接](https://github.com/rushiranpise/Shizuku-Next) [使用教程](https://shizuku.rikka.app/zh-hans/guide/setup)
> 
> <img src="https://wxxsfxyzm.github.io/InstallerX-Revived-Website/ic_launcher.svg" alt="InstallerX Revived" width="16" /> InstallerX Revived下载链接：
> 
> [GitHub](https://github.com/wxxsfxyzm/InstallerX-Revived) [Telegram](https://t.me/installerx_revived)
> 
> 对于小米手机用户，InstallerX Revived的Shizuku权限设置好后，建议在文件管理app中，长按apk文件，点击“分享-InstallerX Revived”进行安装

### Google Webview（Android 5-9）

内核版本：

| Android | Webview |
| --- | --- |
| Android 5 | Chromium 95 |
| Android 6 | Chromium 106 |
| Android 7 | Chromium 119 |
| Android 8/9 | Chromium 138 |

下载链接：[GitHub](https://github.com/n7n8/ah-browser-fragmentation/releases/tag/Google) [123网盘](https://www.123pan.com/s/OuOKVv-lbw63.html)

### Huawei Webview

> [!NOTE]
> 适用范围：不内置 GMS 框架、搭载 EMUI 或 HarmonyOS 2/3/4 的华为手机

内核版本：Chromium 132

下载链接：[GitHub](https://github.com/n7n8/ah-browser-fragmentation/releases/tag/Huawei(EMUI))
[Telegram](https://t.me/kkdx10)

> [!IMPORTANT]
> 注意：安装新版 Huawei Webview apk 之前，建议先安装新版 Huawei Trichrome Library apk！

> [!WARNING]
> versionCode 为 25011、25023 的`com.huawei.triwebviewlib`由于 **共享库版本号** 完全相同（170004310），导致多个 Chromium 132 内核的 Huawei Trichrome Library 无法共存！
> 
> 需要留意你的手机有没有多余的 Huawei Trichrome Library
> 
> 获得 Huawei Webview 的版本
>
> （记下看到的 共享库版本号 ①）
> 
> ```
> adb shell pm dump com.huawei.webview | grep version
> ```
> 
> 获得 TrichromeLibrary 的版本
>
> （记下看到的 共享库版本号 ②）
> 
> ```
> adb shell dumpsys package|grep name:com
> ```
> 
> 卸载多余的 Huawei Trichrome Library
>
> （留意 共享库版本号，只需要卸载“②有出现且①没有出现”的 共享库版本号 相关的 Trichrome Library，或同 **共享库版本号**，但为较旧 versionCode 的 Trichrome Library！）
>
> 以`com.huawei.triwebviewlib_170004310`为例：
> 
> ```
> adb shell pm uninstall com.huawei.triwebviewlib_170004310
> ```

### Huawei Webview（Android 7-9）

内核版本：Chromium 114

下载链接：[APKMirror](https://www.apkmirror.com/apk/huawei/huawei-webview-2/huawei-webview-114-0-4-327-release/) [apkz](https://www.apkz.com/app/com.huawei.webview) [123网盘](https://www.123pan.com/s/OuOKVv-Sbw63.html)

### Hihonor Webview

> [!NOTE]
> 适用范围：不内置 GMS 框架的（非华为子品牌）荣耀手机

内核版本：Chromium 116

下载链接：[GitHub](https://github.com/n7n8/ah-browser-fragmentation/releases/tag/Honor)

### Amazon Webview

下载链接：[APKMirror](https://www.apkmirror.com/apk/amazon-mobile-llc/amazon-system-webview/)

### AOSP Webview（部分）

LineageOS Webview：[APKMirror](https://www.apkmirror.com/apk/lineageos/android-system-webview-2/)

---
### 💡后话

<details>
   <summary>
      详细展开
   </summary>
   
   （以下写于2026-11-11）
   
   假设某台手机只能升级到Android 13。
   
   如果只随OTA升级系统Webview：Chromium停在101~103左右；

   如果随应用商店（无论是不是Google Play）升级系统Webview：现在已经可以升级至Chromium 156左右。
   
   浏览器内核版本已经相差几年。

   因此，可以见到运行Android 11-13的旧手机，用骁龙865处理器，现在也够用，但是预装的Webview可能还是两位数的，有部分现代网页兼容不了，而更新系统Webview后就不会这样。这就是我做这个教程的意义。

</details>
