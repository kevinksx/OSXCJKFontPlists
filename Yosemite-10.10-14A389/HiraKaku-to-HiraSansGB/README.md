该资料夹包含修改过的Yosemite字体回退档案，<br>
适用范围从Developer Preview 5起、已知其可用于Yosemite正式版14A389。<br>

字体回退档案需置于该目录、且继承该目录本身的权限设定：<br>
> /System/Library/Frameworks/CoreText.framework/Versions/A/Resources<br>

可以藉由如下自动化指令将字体回退档案自动下载到正确的位置、并自动配置正确的系统级档案权限：<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/HiraKaku-to-HiraSansGB/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/HiraKaku-to-HiraSansGB/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

该组字体回退档案包含如下设定:<br>

- OS X 简体中文介面语系使用 Hiragino Sans GB 作为介面字体。<br>
- OS X 繁体中文介面语系使用 Hiragino Kaku Gothic Pro 作为介面字体。<br>

您需确认：<br>

1. 所有上述字型档案均需置入「/System/Library/Fonts/」资料夹以内。<br>
2. 所有上述字型档案均需继承「/System/Library/Fonts/」资料夹本身的权限设定，不可简单使用chmod设定755权限了事。<br>

这两点可以藉由如下Terminal指令自动完成：<br>
<pre><code>sudo cp "/Library/Fonts/Hiragino Sans GB W3.otf" "/System/Library/Fonts/Hiragino Sans GB W3.otf"
sudo cp "/Library/Fonts/Hiragino Sans GB W6.otf" "/System/Library/Fonts/Hiragino Sans GB W6.otf"
sudo cp "/Library/Fonts/ヒラギノ角ゴ Pro W3.otf" "/System/Library/Fonts/ヒラギノ角ゴ Pro W3.otf"
sudo cp "/Library/Fonts/ヒラギノ角ゴ Pro W6.otf" "/System/Library/Fonts/ヒラギノ角ゴ Pro W6.otf"</code></pre>

请且仅请在您了解这些档案的适用目的之后再考虑下载这些档案。<br>

==============================================================================<br>

該資料夾包含修改過的Yosemite字體回退檔案，<br>
適用範圍從Developer Preview 5起、已知其可用於Yosemite正式版14A389。<br>

字體回退檔案需置於該目錄、且繼承該目錄本身的權限設定:<br>
> /System/Library/Frameworks/CoreText.framework/Versions/A/Resources<br>

可以藉由如下自動化指令將字體回退檔案自動下載到正確的位置、並自動配置正確的系統級檔案權限：<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/HiraKaku-to-HiraSansGB/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/HiraKaku-to-HiraSansGB/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

該組字體回退檔案包含如下設定:<br>

- OS X 簡體中文介面語系使用 Hiragino Sans GB 作為介面字體。<br>
- OS X 繁體中文介面語系使用 Hiragino Kaku Gothic Pro 作為介面字體。<br>

您需確認：<br>

1. 所有上述字型檔案均需置入「/System/Library/Fonts/」資料夾以內。<br>
2. 所有上述字型檔案均需繼承「/System/Library/Fonts/」資料夾本身的權限設定，不可簡單使用chmod設定755權限了事。<br>

這兩點可以藉由如下Terminal指令自動完成：<br>
<pre><code>sudo cp "/Library/Fonts/Hiragino Sans GB W3.otf" "/System/Library/Fonts/Hiragino Sans GB W3.otf"
sudo cp "/Library/Fonts/Hiragino Sans GB W6.otf" "/System/Library/Fonts/Hiragino Sans GB W6.otf"
sudo cp "/Library/Fonts/ヒラギノ角ゴ Pro W3.otf" "/System/Library/Fonts/ヒラギノ角ゴ Pro W3.otf"
sudo cp "/Library/Fonts/ヒラギノ角ゴ Pro W6.otf" "/System/Library/Fonts/ヒラギノ角ゴ Pro W6.otf"</code></pre>


請且僅請在您了解這些檔案的適用目的之後再考慮下載這些檔案。<br>

==============================================================================<br>

This folder contains customized font fallback plist files of Yosemite since Developer Preview 5 till RTM build 14A389.<br>

Font Fallback plists files should be placed in the following folder and inherit permission settings from it:<br>
> /System/Library/Frameworks/CoreText.framework/Versions/A/Resources<br>

You could use following Terminal commands to download and place them well with correct System Permission settings unless you have no access to GitHub:<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/HiraKaku-to-HiraSansGB/CTPresetFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/CTPresetFallbacks.plist
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/Yosemite-10.10-14A389/HiraKaku-to-HiraSansGB/DefaultFontFallbacks.plist\?raw\=true -o /System/Library/Frameworks/CoreText.framework/Versions/A/Resources/DefaultFontFallbacks.plist</code></pre>

They are customized for the following setting:<br>

- Simplified Chinese GUI of OS X uses Hiragino Sans GB as its GUI font.<br>
- Traditional Chinese GUI of OS X uses Hiragino Kaku Gothic Pro as its GUI font.<br>

You should make sure:<br>

1. All of those fonts I mentioned above must be placed into "/System/Library/Fonts/" folder:<br>
2. All of those fonts I mentioned above should inherit permission settings from "/System/Library/Fonts/", NOT just simple 755.<br>

You could get these two things done by using following Terminal commands:<br>
<pre><code>sudo cp "/Library/Fonts/Hiragino Sans GB W3.otf" "/System/Library/Fonts/Hiragino Sans GB W3.otf"
sudo cp "/Library/Fonts/Hiragino Sans GB W6.otf" "/System/Library/Fonts/Hiragino Sans GB W6.otf"
sudo cp "/Library/Fonts/ヒラギノ角ゴ Pro W3.otf" "/System/Library/Fonts/ヒラギノ角ゴ Pro W3.otf"
sudo cp "/Library/Fonts/ヒラギノ角ゴ Pro W6.otf" "/System/Library/Fonts/ヒラギノ角ゴ Pro W6.otf"</code></pre>

You should download files only if you know what they are and what they should be used for.<br>
