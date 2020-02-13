# Introduction / 简介
### English
Chromium-EyeProtect is a fork of [Chromium Browser](https://www.chromium.org/Home).

This fork was intended to rollback said "Refresh UI" to the legacy UI, which I think is nice and productive.

I know everyone have his/her own view about what UI is beautiful, therefore, if you like this project, I'd like to provide you with these patches or even pre-built binaries to "protect our eyes".

If you don't like it, you may simply close this page.


You can check [My Blog(Chinese)](https://blog.berd.moe/archives/chromium-eyeprotect/) for extra descriptions. To setup API Keys, please refer to [This Article](https://www.chromium.org/developers/how-tos/api-keys) or [My Blog(Chinese)](https://blog.berd.moe/archives/chromium-setup-api-keys/).

### 中文
Chromium-EyeProtect 是 [Chromium Browser](https://www.chromium.org/Home) 的一个分支.

该分支意在将所谓的 "Refresh UI" 回滚到我认为好看且高效的传统 UI

我知道每个人关于什么UI好看的观点各部相同, 因此, 如果你喜欢这个项目, 我很乐意给你提供这些补丁或者预编译的安装包来 "护眼".

如果你不喜欢这个项目, 你可以直接关闭本页面, **不需要尝试把你的观点强加在别人身上**.


你可以访问 [我的博客](https://blog.berd.moe/archives/chromium-eyeprotect/) 来得到更多信息, 关于 API Key 的配置请参考 [本文](https://blog.berd.moe/archives/chromium-setup-api-keys/).

# Recommended Flags Settings / 推荐的Flags设置
* __#eye-protction__ = *enabled*
* __#tab-hover-cards__ = *disabled*
* __#simplify-https-indicator__ = *disabled*
* __#omnibox-ui-hide-steady-state-url-scheme__ = *disabled*
* __#omnibox-ui-hide-steady-state-url-trivial-subdomains__ = *disabled*
* __#omnibox-ui-hide-steady-state-url-path-query-and-ref__ = *disabled*

# Pre-Built Binaries / 预编译安装包
- OneDrive: [Link](https://fengberd-my.sharepoint.com/:f:/g/personal/admin_berd_moe/EgfAnbvVaB5KucXzZ7VXSMwB_1c1EFyokgcc2m8ZUb3m2A?e=YuAFcz)
	- Builds for v77 and later, Windows and Linux.
- 百度云(BaiduCloud): [Link](https://pan.baidu.com/s/1o_jbSlPvJ9jyC-AnebLFjA)
	- Chinese cloud drive.
	- 提取码(Passcode): `edfb`
	- Including v74,v75,v77 and later, Windows and Linux.

# Building / 构建
Patches here are meant to be applied to Chromium official source directly.
The following steps shows you how to start from zero.
 1. Get chromium code following [This Guide](https://www.chromium.org/developers/how-tos/get-the-code)
 2. Checkout to the target version, each version in chromium repository have an corresponding tag
 3. Move to ___src___ directory and apply patches using `git apply <Patch Name>`
 4. Sync dependencies using `gclient sync -D --with_branch_heads --with_tags --force`
 5. Use `gn args out/Release` to modify build parameters
 6. In some scenarios, the gn won't wait for your editor to exit, so you have to run `gn gen out/Release` again after you modified parameters
 7. Finally, you can use `autoninja -C out/Release chrome` to build chromium
 8. If you want to get an installer (in windows), use `autoninja -C out/Release mini_installer` and pick up `mini_installer.exe` in Release directory.

# Android / 安卓版
### English
Due to the lack of sync support, I may not patch the Android Chromium.
Related News:
 - [https://www.androidpolice.com/2017/01/24/google-shuts-off-chrome-sync-api-third-party-browsers-android-citing-security-vulnerability/](https://www.androidpolice.com/2017/01/24/google-shuts-off-chrome-sync-api-third-party-browsers-android-citing-security-vulnerability/)
 - [https://www.ghacks.net/2017/01/25/google-shuts-down-chrome-sync-for-third-party-browsers-on-android/](https://www.ghacks.net/2017/01/25/google-shuts-down-chrome-sync-for-third-party-browsers-on-android/)

### 中文
由于缺少同步功能的支持, 我可能不会去修改 Android Chromium
相关新闻:
 - [https://www.androidpolice.com/2017/01/24/google-shuts-off-chrome-sync-api-third-party-browsers-android-citing-security-vulnerability/](https://www.androidpolice.com/2017/01/24/google-shuts-off-chrome-sync-api-third-party-browsers-android-citing-security-vulnerability/)
 - [https://www.ghacks.net/2017/01/25/google-shuts-down-chrome-sync-for-third-party-browsers-on-android/](https://www.ghacks.net/2017/01/25/google-shuts-down-chrome-sync-for-third-party-browsers-on-android/)

![在写了在写了](https://raw.githubusercontent.com/fengberd/Chromium-EyeProtect/gugu/gugu.jpg)
