### 1. Google Webview

1. 各大国产厂商（小米、vivo、OPPO、荣耀）的新机（荣耀低端机除外）都预装了谷歌官方的Android System Webview。
2. 厂商的 OEM 应用商店都不提供 Android System Webview 的更新。（例外：三星能在系统设置中更新系统Webview）
3. 由于“CN-Flag GMS”的限制，即使用户自己折腾并安装了 Google Play 商店，系统仍然不会自动更新Android System Webview。
4. 由于Google的Android系统变动，Google Play 商店现在已经搜索不到 Android System Webview 的应用界面，转移到“Google 设置>系统服务”。
5. 系统设置中的“Google 设置（Activity名称：com.google.android.gms.app.settings.GoogleSettingsIALink）”在这些定制 OEM 系统中可能被故意隐藏（特别点名 HyperOS 隐藏了它），而“Google 设置>系统服务”正是现在手动检查Android System Webview更新的主要入口。

结论：对90%以上的用户来说，Webview更新被锁死到不及时（估计每年低于4次）的OTA更新中。这导致新版Google Webview（最新版本，主要是Google Play用户）、次新版Google Webview（落后5-15个版本，主要是依靠OTA升级Webview的新手机）、老版本Webview（落后20个版本以上，存在于老机型、低端机型）同时存在

### 2. Huawei Webview
EMUI、HarmonyOS 2/3/4 使用Huawei Webview，最高Chromium版本为M114

3、MagicOS初期的荣耀手机用的是Hihonor Webview，最高Chromium版本约为M116[参见](https://club.honor.com/cn/thread-29317614-1-1.html)

4、搭载OriginOS的vivo手机可能安装了vivo system Webview（与默认的Google Webview并存，vivo system Webview非默认）

结论：对于预装Google WebView的中国大陆Android设备，其WebView版本与Android版本存在强烈的正相关性；虽然新发布的小米/vivo/OPPO/荣耀手机均内置Google Webview，但旧手机可能残存有老Chromium的Huawei Webview、Hihonor Webview，更有无数已停更OTA的手机的Google Webview没有及时更新
