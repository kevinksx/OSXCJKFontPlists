该资料夹包含修改过的Yosemite字体回退档案，<br>
适用范围从Developer Preview 5起、已知其可用于Yosemite正式版14D131。<br>

字体回退档案需置于该目录、且继承该目录本身的权限设定:<br>
- /System/Library/Frameworks/CoreText.framework/Versions/A/Resources<br>

可以藉由如下自动化指令将字体回退档案自动下载到正确的位置、并自动配置正确的系统级档案权限：<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/SourceHanSansUI/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/SourceHanSansUI/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

该组字体回退档案包含如下设定:<br>

- OS X 简体中文介面语系使用 Source Han Sans UI SC 作为介面字体。<br>
- OS X 繁体中文介面语系使用 uses Source Han Sans UI TC 作为介面字体。<br>
- OS X 韩文介面语系使用 Source Han Sans UI K 作为介面字体。<br>
- OS X 日文介面语系使用 Source Han Sans UI J 作为介面字体。<br>

思源黑体UI（Source Han Sans UI）相关资讯见此：<br>
- https://github.com/ShikiSuen/SourceHanSansUI<br>

您在使用该组字体回退档案时，有义务下载您所选择的编译分支当中的全部字体档案（而不是仅下载您所偏好的语言）。<br>

如果您下载来的档案是诸如zip之类的压缩格式，您有义务在使用之前对其进行解压缩操作。<br>

您可以藉由如下自动化指令将字体档案自动解压缩下载到正确的位置、并自动配置正确的系统级档案权限：<br>
<pre><code>curl -L https://github.com/ShikiSuen/SourceHanSansUI/raw/master/SourceHanSansUI-SuperOTC.zip\?raw\=true | bsdtar -xvf-
sudo cp SourceHanSansUI.ttc /Library/Fonts
sudo chown root:wheel /Library/Fonts/SourceHanSansUI.ttc
sudo chmod 644 /Library/Fonts/SourceHanSansUI.ttc</code></pre>

在套用该组档案之前，您需先确认：<br>

1. 所有上述字型档案均需置入「/System/Library/Fonts/」或「/Library/Fonts/」资料夹以内。<br>
2. 所有上述字型档案均需設定权限为「chown root:wheel」+「chmod 644」。<br>
（其实用sudo指令摆入目标资料夹即可纠正权限；chmod必须搭配chown使用）<br>

请且仅请在您了解这些档案的适用目的之后再考虑下载这些档案。<br>

==============================================================================<br>

該資料夾包含修改過的Yosemite字體回退檔案，<br>
適用範圍從Developer Preview 5起、已知其可用於Yosemite正式版14D131。<br>

字體回退檔案需置於該目錄、且繼承該目錄本身的許可權設定:<br>
- /System/Library/Frameworks/CoreText.framework/Versions/A/Resources<br>

可以藉由如下自動化指令將字體回退檔案自動下載到正確的位置、並自動配置正確的系統級檔案許可權：<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/SourceHanSansUI/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/SourceHanSansUI/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

該組字體回退檔案包含如下設定:<br>

- OS X 簡體中文介面語系使用 Source Han Sans UI SC 作為介面字體。<br>
- OS X 繁體中文介面語系使用 uses Source Han Sans UI TC 作為介面字體。<br>
- OS X 韓文介面語系使用 Source Han Sans UI K 作為介面字體。<br>
- OS X 日文介面語系使用 Source Han Sans UI J 作為介面字體。<br>

思源黑體UI（Source Han Sans UI）相關資訊見此：<br>
- https://github.com/ShikiSuen/SourceHanSansUI<br>

您在使用該組字體回退檔案時，有義務下載您所選擇的編譯分支當中的全部字體檔案（而不是僅下載您所偏好的語言）。<br>

如果您下載來的檔案是諸如zip之類的壓縮格式，您有義務在使用之前對其進行解壓縮操作。<br>

您可以藉由如下自動化指令將字體檔案自動解壓縮下載到正確的位置、並自動配置正確的系統級檔案許可權：<br>
<pre><code>curl -L https://github.com/ShikiSuen/SourceHanSansUI/raw/master/SourceHanSansUI-SuperOTC.zip\?raw\=true | bsdtar -xvf-
sudo cp SourceHanSansUI.ttc /Library/Fonts
sudo chown root:wheel /Library/Fonts/SourceHanSansUI.ttc
sudo chmod 644 /Library/Fonts/SourceHanSansUI.ttc</code></pre>

在套用該組檔案之前，您需先確認：<br>

1. 所有上述字型檔案均需置入「/System/Library/Fonts/」或「/Library/Fonts/」資料夾以內。<br>
2. 所有上述字型檔案均需設定許可權為「chown root:wheel」+「chmod 644」。<br>
（其實用sudo指令擺入目標資料夾即可糾正許可權；chmod必須搭配chown使用）<br>

請且僅請在您瞭解這些檔案的適用目的之後再考慮下載這些檔案。<br>

==============================================================================<br>

This folder contains customized font fallback plist files of Yosemite since Developer Preview 5 till RTM build 14D131.<br>

Font Fallback plists files should be placed in the following folder and inherit permission settings from it:<br>
- /System/Library/Frameworks/CoreText.framework/Versions/A/Resources<br>

You could use following Terminal commands to download and place them well with correct System Permission settings unless you have no access to GitHub:<br>

<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/SourceHanSansUI/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/SourceHanSansUI/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

They are customized for the following setting:<br>

- Simplified Chinese GUI of OS X uses Source Han Sans UI SC as its GUI font.<br>
- Traditional Chinese GUI of OS X uses Source Han Sans UI TC as its GUI font.<br>
- Korean GUI of OS X uses Source Han Sans UI K as its GUI font.<br>
- Japanese GUI of OS X uses Source Han Sans UI J as its GUI font.<br>

For more intel about Source Han Sans UI, please visit:<br>
- https://github.com/ShikiSuen/SourceHanSansUI<br>

You should always install all files of a build with this set of plists (not just download the version of you preferred language only).<br>

You have responsibility to extract them if they are compressed zip package.<br>

You could use following Terminal commands to download and place the font well with correct System Permission settings unless you have no access to GitHub:<br>
<pre><code>curl -L https://github.com/ShikiSuen/SourceHanSansUI/raw/master/SourceHanSansUI-SuperOTC.zip\?raw\=true | bsdtar -xvf-
sudo cp SourceHanSansUI.ttc /System/Library/Fonts
sudo chown root:wheel /System/Library/Fonts/SourceHanSansUI.ttc
sudo chmod 644 /System/Library/Fonts/SourceHanSansUI.ttc</code></pre>

You should make sure following things have done before applying this set of font fallback plists:<br>

1. All of those fonts I mentioned above must be placed into "/System/Library/Fonts/" or "/Library/Fonts/" folder,<br>
2. All of those fonts I mentioned above should use this permission configuration: "chown root:wheel" + "chmod 644".<br>
(use sudo per file operation could get the permission settings fixed automatically.)<br>
(you should always use chmod with chown together.)<br>

You should download files only if you know what they are and what they should be used for.<br>
