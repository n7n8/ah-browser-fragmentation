1. 各大国产厂商（小米、vivo、OPPO、荣耀）的新机（荣耀低端机除外）都预装了谷歌官方的Android System Webview。
2. 厂商的 OEM 应用商店都不提供 Android System Webview 的更新。（例外：三星能在系统设置中更新系统Webview）
3. 由于“CN-Flag GMS”的限制，即使用户自己折腾并安装了 Google Play 商店，系统仍然不会自动更新Android System Webview。
4. 由于Google的Android系统变动，Google Play 商店现在已经搜索不到 Android System Webview 的应用界面，转移到“Google 设置>系统服务”。
5. 系统设置中的“Google 设置（Activity名称：com.google.android.gms.app.settings.GoogleSettingsIALink）”在这些定制 OEM 系统中可能被故意隐藏（特别点名 HyperOS 隐藏了它），而“Google 设置>系统服务”正是现在手动检查Android System Webview更新的主要入口。

结论：对90%以上的用户来说，Webview更新被锁死到不及时（估计每年低于4次）的OTA更新中
