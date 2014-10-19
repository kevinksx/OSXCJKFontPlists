This folder contains customized font fallback plist files of Yosemite since Developer Preview 5 till RTM build 14A389.<br>
They are customized for the following setting:

Simplified Chinese GUI of OS X uses Source Han Sans SC as its GUI font.<br>
Traditional Chinese GUI of OS X uses Source Han Sans TC as its GUI font.<br>
Korean GUI of OS X uses Source Han Sans K as its GUI font.<br>
Japanese GUI of OS X uses Source Han Sans as its GUI font.

Only these Source Han Sans builds are applicable with this set of plists:<br>
https://github.com/adobe-fonts/source-han-sans/tree/release/SuperOTC <br>
https://github.com/adobe-fonts/source-han-sans/tree/release/OTC <br>
https://github.com/adobe-fonts/source-han-sans/tree/release/OTF <br>

You should always install all files of a build, not just the version of you preferred language.<br>
You have responsibility to extract them if they are compressed zip package.<br>

You should make sure:<br>
1. All of those fonts I mentioned above must be placed into "/System/Library/Fonts/" folder,<br>
2. All of those fonts I mentioned above should inherit permission settings from "/System/Library/Fonts/", NOT just simple 755.<br>

You should download files only if you know what they are and what they should be used for.<br>
