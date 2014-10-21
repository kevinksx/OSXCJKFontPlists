OSX CJK Font-Fallback Plists 專頁
=========================

本專頁的資料主要和 OS X 中日韓介面字體修改有關。<br>

1. 請在取用具體的資料之前確保自己先了解其用途。<br>
2. <u>敝专页以原生繁体中文撰写</u>，<u>仅习惯阅读简体中文的访客们请善用Chrome的同文堂扩展</u>。<br>
3. 敝專頁的所有方法均要求當事電腦可以連線到GitHub。<br>
4. 敝專頁目前暫時只服務 OS X Yosemite 使用者群體。<br>
5. 敝專頁所提及的全部分頁的網址都會隨該大版本OS X的次版本更新而變動。<br>

同時修改多個區域的預設介面顯示字體的重要性
--------
假設你在用中文優先顯示為系統介面語系的時候，<br>
如果系統字體的優先顯示順序被你設定為「簡體中文/繁體中文/日語/英文」的話，<br>
某些沒有中文但有日文或繁體中文的軟體則不會遵循簡體中文的字體顯示設定。<br>
所以有時候不只您常用的語系的預設介面字體需要修改。<br>


如何恢復原廠字體設定
--------

在修改字體之前，需要先知道自己在字體修改失敗、或者後悔時所能做的。<br>
該恢復過程可以便於檢查自己所遇到的錯誤究竟是否與字體修改過程本身有關。<br>

如果華文黑體已經自系統內移除的話，則請在恢復原廠字體回退設定檔案之前、先恢復華文黑體：<br>
https://github.com/ShikiSuen/OSXCJKFontPlists/tree/master/FactorialSTHeitiBackup<br>
（否則會出現無法預測的問題）<br>

關於恢復原廠字體回退設定檔案的方法請參見該分頁：<br>
https://github.com/ShikiSuen/OSXCJKFontPlists/tree/master/Yosemite-10.10-14A389/FactorialPlists<br>

字體修改方案篇
--------

###修改前須知###

請在套用對應分組的字體回退設定檔案修改方案之前，先確保這兩點：<br>

1. 所有上述字型檔案均需置入「/System/Library/Fonts/」資料夾以內。<br>
2. 所有上述字型檔案均需繼承「/System/Library/Fonts/」資料夾本身的權限設定以糾正權限。<br>
（其實用sudo指令擺入該資料夾即可糾正權限；凡是僅基於chmod的方法都是隔靴搔癢）<br>
（我很難想像在脫離chown的情況下如何討論chmod設定權限的可行性）<br>

不出意外的話，下述各方案所涉分頁當中都寫明了各自的、均藉由Terminal實現這兩點的方法。<br>

您可能希望在套用對應分組的字體回退設定檔案修改方案之後移除華文黑體：<br>
<pre><code>killall Finder
sudo rm –Rf "/System/Library/Fonts/STHeiti Light.ttc"
sudo rm –Rf "/System/Library/Fonts/STHeiti Medium.ttc"
sudo rm –Rf "/System/Library/Fonts/STHeiti Thin.ttc"
sudo rm –Rf "/System/Library/Fonts/STHeiti UltraLight.ttc"
sudo rm –Rf "/Library/Fonts/华文细黑.ttf"
sudo rm –Rf "/Library/Fonts/华文黑体.ttf"</code></pre>
這樣可以防止華文黑體在某些應用程式介面當中詐屍還魂。<br>
（關於華文黑體的恢復方法請參見上文，不再贅述）<br>

最後必須緊接著清理系統的字體快取/緩存，並緊接著重新開機：<br>
<pre><code>sudo atsutil databases -remove
sudo reboot</code></pre>

修改字體的所有步驟，均需行雲流水、一次完成。<br>
故請在修改之前將所有工作存檔、並將無關的應用全部關閉。<br>

###【實例】修改系統中文介面字體為冬青黑體###

簡體中文介面語系自然是要使用冬青黑體簡體中文（ヒラギノ角ゴ 簡体中文），<br>
但鑑於不同繁體中文的用戶偏好，我們給出了兩種方案：<br>

1. 繁體中文語系亦使用冬青黑體簡體中文做為介面字體：<br>
https://github.com/ShikiSuen/OSXCJKFontPlists/tree/master/Yosemite-10.10-14A389/HiraginoSansGB<br>
2. 繁體中文語系使用冬青黑體Pro（ヒラギノ角ゴ Pro）：<br>
https://github.com/ShikiSuen/OSXCJKFontPlists/tree/master/Yosemite-10.10-14A389/HiraKaku-to-HiraSansGB<br>

請務必先完成具體分頁的說明當中「在套用該組檔案之前，您需先確認」處的要求，<br>
再套用配套的字體回退設定檔案。<br>

###【實例】修改系統簡繁日韓介面字體為思源黑體###

鑑於上文所述之原因，簡繁日韓文都需要改成思源黑體。<br>
https://github.com/ShikiSuen/OSXCJKFontPlists/tree/master/Yosemite-10.10-14A389/SHS-LSR<br>
請務必在套用字體回退設定檔案之前、<br>
將字體檔案自動解壓縮下載到正確的位置，並確保其權限正確。<br>
（根據該分頁當中給出的Terminal指令去做就可以了）

寫在最後
--------
敝專頁歸屬此Git專案進行維護：<br>
https://github.com/ShikiSuen/OSXCJKFontPlists<br>
如果大家發現問題的話（無論是網頁說明問題，還是分頁當中提到的檔案問題），<br>
歡迎藉由該Git專案進行提報。<br>
