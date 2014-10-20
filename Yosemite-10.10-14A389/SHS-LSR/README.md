该资料夹包含修改过的Yosemite字体回退档案，<br>
适用范围从Developer Preview 5起、已知其可用于Yosemite正式版14A389。<br>

字体回退档案需置于该目录、且继承该目录本身的权限设定:<br>
「/System/Library/Frameworks/CoreText.framework/Versions/A/Resources」<br>
可以藉由如下自动化指令将字体回退档案自动下载到正确的位置（不包含额外设定权限的步骤）：<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/SHS-LSR/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/SHS-LSR/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

该组字体回退档案包含如下设定:<br>

OS X 简体中文介面语系使用 Source Han Sans SC 作为介面字体。<br>
OS X 繁体中文介面语系使用 uses Source Han Sans TC 作为介面字体。<br>
OS X 韩文介面语系使用 Source Han Sans K 作为介面字体。<br>
OS X 日文介面语系使用 Source Han Sans 作为介面字体。<br>

思源黑体（Source Han Sans）仅如下编译分支可搭配该组字体回退档案使用：<br>
https://github.com/adobe-fonts/source-han-sans/tree/release/SuperOTC <br>
https://github.com/adobe-fonts/source-han-sans/tree/release/OTC <br>
https://github.com/adobe-fonts/source-han-sans/tree/release/OTF <br>

您在使用该组字体回退档案时，有义务下载您所选择的编译分支当中的全部字体档案（而不是仅下载您所偏好的语言）。<br>
如果您下载来的档案是诸如zip之类的压缩格式，您有义务在使用之前对其进行解压缩操作。<br>

您需确认：<br>
1. 所有上述字型档案均需置入「/System/Library/Fonts/」资料夹以内。<br>
2. 所有上述字型档案均需继承「/System/Library/Fonts/」资料夹本身的权限设定，不可简单使用chmod设定755权限了事。<br>

请且仅请在您了解这些档案的适用目的之后再考虑下载这些档案。<br>

==============================================================================<br>

該資料夾包含修改過的Yosemite字體回退檔案，<br>
適用範圍從Developer Preview 5起、已知其可用於Yosemite正式版14A389。<br>

字體回退檔案需置於該目錄、且繼承該目錄本身的權限設定:<br>
「/System/Library/Frameworks/CoreText.framework/Versions/A/Resources」<br>
可以藉由如下自動化指令將字體回退檔案自動下載到正確的位置（不包含額外設定權限的步驟）：<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/SHS-LSR/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/SHS-LSR/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

該組字體回退檔案包含如下設定:<br>

OS X 簡體中文介面語系使用 Source Han Sans SC 作為介面字體。<br>
OS X 繁體中文介面語系使用 uses Source Han Sans TC 作為介面字體。<br>
OS X 韓文介面語系使用 Source Han Sans K 作為介面字體。<br>
OS X 日文介面語系使用 Source Han Sans 作為介面字體。<br>

思源黑體（Source Han Sans）僅如下編譯分支可搭配該組字體回退檔案使用：<br>
https://github.com/adobe-fonts/source-han-sans/tree/release/SuperOTC <br>
https://github.com/adobe-fonts/source-han-sans/tree/release/OTC <br>
https://github.com/adobe-fonts/source-han-sans/tree/release/OTF <br>

您在使用該組字體回退檔案時，有義務下載您所選擇的編譯分支當中的全部字體檔案（而不是僅下載您所偏好的語言）。<br>
如果您下載來的檔案是諸如zip之類的壓縮格式，您有義務在使用之前對其進行解壓縮操作。<br>

您需確認：<br>
1. 所有上述字型檔案均需置入「/System/Library/Fonts/」資料夾以內。<br>
2. 所有上述字型檔案均需繼承「/System/Library/Fonts/」資料夾本身的權限設定，不可簡單使用chmod設定755權限了事。<br>

請且僅請在您了解這些檔案的適用目的之後再考慮下載這些檔案。<br>

==============================================================================<br>

This folder contains customized font fallback plist files of Yosemite since Developer Preview 5 till RTM build 14A389.<br>

Font Fallback plists files should be placed in the following folder and inherit permission settings from it:<br>
"/System/Library/Frameworks/CoreText.framework/Versions/A/Resources"<br>
You could use following Terminal commands to download and place them well unless you have no access to GitHub:<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/SHS-LSR/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/SHS-LSR/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

They are customized for the following setting:<br>

Simplified Chinese GUI of OS X uses Source Han Sans SC as its GUI font.<br>
Traditional Chinese GUI of OS X uses Source Han Sans TC as its GUI font.<br>
Korean GUI of OS X uses Source Han Sans K as its GUI font.<br>
Japanese GUI of OS X uses Source Han Sans as its GUI font.

Only these Source Han Sans builds are applicable with this set of plists:<br>
https://github.com/adobe-fonts/source-han-sans/tree/release/SuperOTC <br>
https://github.com/adobe-fonts/source-han-sans/tree/release/OTC <br>
https://github.com/adobe-fonts/source-han-sans/tree/release/OTF <br>

You should always install all files of a build with this set of plists (not just download the version of you preferred language only).<br>
You have responsibility to extract them if they are compressed zip package.<br>

You should make sure:<br>
1. All of those fonts I mentioned above must be placed into "/System/Library/Fonts/" folder,<br>
2. All of those fonts I mentioned above should inherit permission settings from "/System/Library/Fonts/", NOT just simple 755.<br>

You should download files only if you know what they are and what they should be used for.<br>
