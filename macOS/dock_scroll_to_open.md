# 鼠标滚轮控制 Dock 文件夹展开

## 用鼠标滚轮打开或者关闭 Dock 文件夹的展开预览

启用

	defaults write com.apple.dock scroll-to-open -bool TRUE && killall Dock

禁用

	defaults write com.apple.dock scroll-to-open -bool False && killall Dock
