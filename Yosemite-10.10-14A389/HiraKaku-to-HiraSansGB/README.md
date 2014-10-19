This folder contains customized font fallback plist files of Yosemite since Developer Preview 5 till RTM build 14A389.
They are customized for the following setting:

Simplified Chinese GUI of OS X uses Hiragino Sans GB as its GUI font.
Traditional Chinese GUI of OS X uses Hiragino Kaku Gothic Pro as its GUI font.

You should make sure:
1. All of those fonts I mentioned above must be placed into "/System/Library/Fonts/" folder,
2. All of those fonts I mentioned above should inherit permission settings from "/System/Library/Fonts/", NOT just simple 755.

You should download files only if you know what they are and what they should be used for.