1、各大国产厂商（小米、vivo、OPPO、荣耀）的新机都预装了谷歌官方的Android System Webview。

​2、厂商的 OEM 应用商店都不提供 Android System Webview 的更新。

​3、由于“CN-Flag GMS”的限制，即使用户自己折腾并安装了 Google Play 商店，系统仍然不会自动更新Android System Webview。

4、由于Google的Android系统变动，Google Play 商店现在已经搜索不到 Android System Webview 的应用界面，转移到“Google 设置>系统服务”。

​5、系统底层中的“Google 设置”在这些定制 OEM 系统（如 HyperOS、OriginOS、ColorOS 等）中经常被故意隐藏，而“Google 设置>系统服务”正是现在检查Android System Webview更新的主要入口。

---

结论：对90%以上的用户来说，Webview更新被锁死到不及时（通常每年低于4次）的OTA更新中


解决方案：如何使用已有apk手动更新Android System Webview？

对于vivo、OPPO、荣耀手机用户，直接安装Android System Webview apk即可

对于小米手机用户，需要确保开启开发者选项、adb调试、USB安装，再通过PC或adb安装器（如[Shizuku](https://github.com/thedjchi/Shizuku)
授权[InstallerX Revived](https://github.com/wxxsfxyzm/InstallerX-Revived)
的组合）安装Webview apk


附注-哪些渠道能更新Android System Webview（✅❎表示，✅表示可更新，❎表示不可更新）？在中国大陆网络条件可用吗（🟢🔴表示，🟢表示可用，🔴表示不可用）？

Google Play：✅🔴

APKMirror：✅🔴

Apkpure：✅🔴

Uptodown：✅🔴

---

华为：❎🟢

荣耀：❎🟢

小米：❎🟢

OPPO：❎🟢

vivo：❎🟢

三星：❎🟢

百度：❎🟢

豌豆荚：❎🟢

腾讯：❎🟢

魅族：❎🟢

Lenovo：❎🟢

---

[安大师](https://www.apkz.com/zh_cn.html)：✅🟢

酷安：（需搜索“Webview”，进入网友分享的网盘链接；官方不上架）🟢

[AppShare](https://app.sharess.cn/)：
（需搜索“Webview”，进入网友分享的网盘链接；可能需要下载app）🟢

---

附注2-各个跟进主线的Android浏览器是否在中国大陆地区服务？

Brave：🔴否

Chrome：🟡不确定（部分品牌应用商店灰色上架）

Ecosia：🔴否

Edge：🟢是

Firefox：🔴否

Opera：🔴否

Vivaldi：🔴否

Yandex：🔴否

XWeb（微信）：🟢是（但这不是浏览器）
