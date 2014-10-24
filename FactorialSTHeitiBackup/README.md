该资料夹包含Yosemite原厂的简繁体中文介面字体档案备份。<br>
若欲恢复系统原厂中文字体、却苦于华文黑体已被刚除，则可自此下载之。<br>

以下四个字型档案请置于「/System/Library/Fonts/」目录之下：<br>

- STHeiti Light.ttc<br>
- STHeiti Medium.ttc<br>
- STHeiti Thin.ttc<br>
- STHeiti UltraLight.ttc<br>

且需继承该目录本身的权限设定。<br>

以下两个字型档案请置于「/Library/Fonts/」目录之下：<br>

- 华文黑体.ttf<br>
- 华文细黑.ttf<br>

且需继承该目录本身的权限设定。<br>

可以藉由如下自动化指令来一次性完成华文黑体的还原工作（请确保可以正常连线到Github）：<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20Light.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti Light.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20Medium.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti Medium.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20Thin.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti Thin.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20UltraLight.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti UltraLight.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/华文细黑.ttf\?raw\=true -o "/Library/Fonts/华文细黑.ttf"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/华文黑体.ttf\?raw\=true -o "/Library/Fonts/华文黑体.ttf"
sudo chown root:wheel "/System/Library/Fonts/STHeiti Light.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti Light.ttc"
sudo chown root:wheel "/System/Library/Fonts/STHeiti Medium.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti Medium.ttc"
sudo chown root:wheel "/System/Library/Fonts/STHeiti Thin.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti Thin.ttc"
sudo chown root:wheel "/System/Library/Fonts/STHeiti UltraLight.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti UltraLight.ttc"
sudo chown root:wheel "/Library/Fonts/华文细黑.ttf"
sudo chmod 644 "/Library/Fonts/华文细黑.ttf"
sudo chown root:wheel "/Library/Fonts/华文细黑.ttf"
sudo chmod 644 "/Library/Fonts/华文细黑.ttf"</code></pre>

请且仅请在您了解这些档案的适用目的之后再考虑下载这些档案。<br>

==============================================================================<br>

該資料夾包含Yosemite原廠的簡繁體中文介面字體檔案備份。<br>
若欲恢復系統原廠中文字體、卻苦於華文黑體已被剛除，則可自此下載之。<br>

以下四個字型檔案請置於「/System/Library/Fonts/」目錄之下：<br>

- STHeiti Light.ttc<br>
- STHeiti Medium.ttc<br>
- STHeiti Thin.ttc<br>
- STHeiti UltraLight.ttc<br>

且需繼承該目錄本身的權限設定。<br>

以下兩個字型檔案請置於「/Library/Fonts/」目錄之下：<br>

- 华文黑体.ttf<br>
- 华文细黑.ttf<br>

且需繼承該目錄本身的權限設定。<br>

可以藉由如下自動化指令來一次性完成華文黑體的還原工作（請確保可以正常連線到Github）：<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20Light.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti Light.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20Medium.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti Medium.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20Thin.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti Thin.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20UltraLight.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti UltraLight.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/华文细黑.ttf\?raw\=true -o "/Library/Fonts/华文细黑.ttf"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/华文黑体.ttf\?raw\=true -o "/Library/Fonts/华文黑体.ttf"
sudo chown root:wheel "/System/Library/Fonts/STHeiti Light.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti Light.ttc"
sudo chown root:wheel "/System/Library/Fonts/STHeiti Medium.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti Medium.ttc"
sudo chown root:wheel "/System/Library/Fonts/STHeiti Thin.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti Thin.ttc"
sudo chown root:wheel "/System/Library/Fonts/STHeiti UltraLight.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti UltraLight.ttc"
sudo chown root:wheel "/Library/Fonts/华文细黑.ttf"
sudo chmod 644 "/Library/Fonts/华文细黑.ttf"
sudo chown root:wheel "/Library/Fonts/华文细黑.ttf"
sudo chmod 644 "/Library/Fonts/华文细黑.ttf"</code></pre>

請且僅請在您瞭解這些檔案的適用目的之後再考慮下載這些檔案。<br>

==============================================================================<br>

This folder contains Factorial STHeiti Font Backup if you want to recover factorial Chinese GUI fonts.<br>

Put following files into "/System/Library/Fonts/" folder:<br>

- STHeiti Light.ttc<br>
- STHeiti Medium.ttc<br>
- STHeiti Thin.ttc<br>
- STHeiti UltraLight.ttc<br>

And these files should inherit permission settings from this folder.<br>

Put following files into "/System/Library/Fonts/" folder:<br>

- 华文黑体.ttf<br>
- 华文细黑.ttf<br>

And these files should inherit permission settings from this folder.<br>

You could use following Terminal commands to do all of these recovery works I mentioned above unless you have no access to GitHub:<br>
<pre><code>sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20Light.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti Light.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20Medium.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti Medium.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20Thin.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti Thin.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/STHeiti%20UltraLight.ttc\?raw\=true -o "/System/Library/Fonts/STHeiti UltraLight.ttc"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/华文细黑.ttf\?raw\=true -o "/Library/Fonts/华文细黑.ttf"
sudo curl -L https://github.com/ShikiSuen/OSXCJKFontPlists/blob/master/FactorialSTHeitiBackup/华文黑体.ttf\?raw\=true -o "/Library/Fonts/华文黑体.ttf"
sudo chown root:wheel "/System/Library/Fonts/STHeiti Light.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti Light.ttc"
sudo chown root:wheel "/System/Library/Fonts/STHeiti Medium.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti Medium.ttc"
sudo chown root:wheel "/System/Library/Fonts/STHeiti Thin.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti Thin.ttc"
sudo chown root:wheel "/System/Library/Fonts/STHeiti UltraLight.ttc"
sudo chmod 644 "/System/Library/Fonts/STHeiti UltraLight.ttc"
sudo chown root:wheel "/Library/Fonts/华文细黑.ttf"
sudo chmod 644 "/Library/Fonts/华文细黑.ttf"
sudo chown root:wheel "/Library/Fonts/华文细黑.ttf"
sudo chmod 644 "/Library/Fonts/华文细黑.ttf"</code></pre>

You should download files only if you know what they are and what they should be used for.<br>