3种基本形式：依赖系统Webview、apk自带内核、动态加载内核

“动态加载内核”不能独立存在，只可能与“依赖系统Webview”（如QQ浏览器、抖音）、“apk自带内核”（如UC浏览器、夸克）中的其一组合，且优先级大于“依赖系统Webview”和“apk自带内核”

---

一•国内篇

①依赖系统Webview

适用范围：部分浏览器app（如Via浏览器）、部分非浏览器app

更新渠道：基本仅依赖系统更新且更新频率低，因此系统Webview碎片化非常严重。关于Webview更新的问题，详见《官方渠道更新系统Webview现状&解决方案》

②apk自带内核

适用范围：部分浏览器app（包括“米ov耀”的OEM浏览器）、少数非浏览器app

更新渠道：通过OEM应用商店更新

③动态加载内核

适用范围：部分浏览器app（如夸克、QQ浏览器、UC浏览器）、部分主流非浏览器app（尤其是超级app，如微信、支付宝、抖音）

更新渠道：通过热更新（Hotfix）或自建 CDN 动态下发/升级浏览器内核，需要重启app生效。这解决了“由于部分人长期不更新apk，因此难以更新浏览器内核”的问题，提高厂商对浏览器内核更新节奏的控制

注：国产浏览器基本不存在 UA 与实际内核版本不符的情况；apk自带内核、动态加载内核可能存在“补丁回溯”，因此部分厂商的定制浏览器内核（如X5）的Chromium版本虽然与Web API挂钩，但不能直接反映其安全状态（注意：旧版Chromium不存在新版Chromium的部分新漏洞）

---

二•国际篇

①依赖系统Webview

适用范围：部分浏览器app、大多数非浏览器app

更新渠道：Android System Webview通过Google Play强制更新；普通用户难以关闭其更新

②apk自带内核

适用范围：大多数主流浏览器app（包括Chrome、Samsung Internet）、少数非浏览器app

更新渠道：Google Play。会受到“用户手动关闭更新”的影响

③动态加载内核

适用范围：无。通过 Google Play 分发的应用不得从外部来源下载可执行代码，因此 Google Play 禁止“动态加载内核”方案

注：Facebook/Instagram模式非常特殊。虽然是分包apk内置的浏览器内核，但是通过Google Play或海外Android手机的特殊系统组件（如Meta App Installer、Meta App Manager、Meta Services）自动更新浏览器内核；Facebook/Instagram模式只局限于这2个app
