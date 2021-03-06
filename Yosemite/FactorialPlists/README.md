该资料夹包含Yosemite原厂字体回退档案。<br>
已知 Developer Preview 5 和 14D131 的原厂字体回退档案都是这一组。<br>

- 如果华文黑体已被刚除，则在您换上原厂字体回退档案之前需要恢复华文黑体。<br>
详情请参见「FactorialSTHeitiBackup」资料夹当中的各类档案：<br>
https://github.com/ShikiSuen/OSXCJKFontPlists/tree/master/FactorialSTHeitiBackup<br>

字体回退档案可在刚刚安装完毕系统之后的该目录下寻获、且继承该目录本身的权限设定：<br>
> /System/Library/Frameworks/CoreText.framework/Versions/A/Resources<br>

可以藉由如下自动化指令自动套用原厂字体回退档案：<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/FactorialPlists/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/FactorialPlists/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

请且仅请在您了解这些档案的适用目的之后再考虑下载这些档案。<br>

==============================================================================<br>

該資料夾包含Yosemite原廠字體回退檔案。<br>
已知 Developer Preview 5 和 14D131 的原廠字體回退檔案都是這一組。<br>

- 如果華文黑體已被剛除，則在您換上原廠字體回退檔案之前需要恢復華文黑體。<br>
詳情請參見「FactorialSTHeitiBackup」資料夾當中的各類檔案：<br>
https://github.com/ShikiSuen/OSXCJKFontPlists/tree/master/FactorialSTHeitiBackup<br>

字體回退檔案可在剛剛安裝完畢系統之後的該目錄下尋獲、且繼承該目錄本身的權限設定：<br>
> /System/Library/Frameworks/CoreText.framework/Versions/A/Resources<br>

可以藉由如下自動化指令自動套用原廠字體回退檔案：<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/FactorialPlists/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/FactorialPlists/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

請且僅請在您了解這些檔案的適用目的之後再考慮下載這些檔案。<br>

==============================================================================<br>

This folder contains Factorial Font Fallback plist files of Yosemite since Developer Preview 5 till RTM build 14D131.<br>

- If STHeiti (factorial Chinese GUI font which looks freaking) had been removed,<br>
you have to recover them before applying factorial font fallback plists to your system.<br>
See folder "FactorialSTHeitiBackup" for further information:<br>
https://github.com/ShikiSuen/OSXCJKFontPlists/tree/master/FactorialSTHeitiBackup<br>

Font Fallback plists files could be fond in the following folder of fresh-installed system:<br>
> /System/Library/Frameworks/CoreText.framework/Versions/A/Resources<br>

You could use following Terminal commands to download and place them well with correct System Permission settings unless you have no access to GitHub:<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/FactorialPlists/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite/FactorialPlists/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo chown root:wheel /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist
sudo chmod 644 /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

You should download files only if you know what they are and what they should be used for.<br>