---
title: 鍵盤按鍵綁定一覽表
nav_order: 9010
has_children: false
parent: 一覽表
---


# 鍵盤按鍵綁定一覽表




## 主題

* [設定腳本](#設定腳本)
* [系統操作](#系統操作)
* [開啟應用程式](#開啟應用程式)
* [視窗操作](#視窗操作)
* [切換](#切換)
* [其他](#其他)
* [螢幕截圖](#螢幕截圖)
* [相關連結](#相關連結)
* [相關專案](#相關專案)




## 設定腳本

| 設定腳本 |
| ------- |
| [gnome-shell-keybind](https://github.com/samwhelp/note-about-anduinos-gnome-shell/blob/gh-pages/_demo/scripts/gnome-shell-keybind) |
| [gnome-shell-adjustment](https://github.com/samwhelp/note-about-anduinos-gnome-shell/tree/gh-pages/_demo/scripts/gnome-shell-adjustment) |




## 系統操作


## 系統操作 / 離開系統

| 按鍵組合           | 功能                   |
| ------------------ | ---------------------- |
| `Alt + Shift + z`  | 關機                   |
| `Alt + Shift + x`  | 登出  |




## 開啟應用程式


## 開啟應用程式 / 透過「應用程式啟動器」

> `org.gnome.desktop.wm.keybindings`

| 按鍵組合    | 功能                                   | 設定項目              |
| ----------- | -------------------------------------- | ------------------------------ |
| `Alt + F1`  | 開啟「應用程式啟動主選單(Arc Menu)」  |
| `Alt + F2`  | 開啟「應用程式啟動器(Runner)」         | `panel-run-dialog`  |




## 開啟應用程式 / 透過「Rofi」

| 按鍵組合           | 功能                            | 執行指令                         |
| ------------------ | ------------------------------- | -------------------------------- |
| `Alt + Shift + d`  | 開啟 Rofi (可用應用程式列表)    | `rofi -show drun -show-icons`    |
| `Alt + Shift + w`  | 開啟 Rofi (已經開啟的視窗列表)  | `rofi -show window -show-icons`  |
| `Alt + Shift + r`  | 開啟 Rofi (可用指令列表)        | `rofi -show run`                 |




## 開啟應用程式 / Terminal

| 按鍵組合           | 功能           | 執行指令          |
| ------------------ | -------------- | ----------------- |
| `Alt + Enter`      | 開啟 Terminal  | `kgx`  |
| `Alt + Shift + a`  | 開啟 Terminal  | `kgx`  |
| `Alt + Ctrl + a`   | 開啟 Terminal  | `gnome-terminal`          |
| `Alt + Shift + t`  | 開啟 Terminal  | `xfce4-terminal`           |
| `Alt + Ctrl + t`   | 開啟 Terminal  | `qterminal`           |


| 按鍵組合           | 功能                     | 執行指令                      |
| ------------------ | ------------------------ | ----------------------------- |
| `Alt + Shift + y`  | 開啟 Drop Down Terminal  | `xfce4-terminal --drop-down`  |




## 開啟應用程式 / 常用的應用程式

| 按鍵組合           | 功能            | 執行指令                         |
| ------------------ | --------------- | -------------------------------- |
| `Alt + Shift + f`  | 開啟檔案管理器  | `nautilus`                         |
| `Alt + Shift + g`  | 開啟檔案管理器  | `thunar`                     |
| `Alt + Shift + e`  | 開啟文字編輯器  | `gnome-text-editor`                       |
| `Alt + Shift + b`  | 開啟網頁瀏覽器  | `firefox --new-tab about:blank`  |
| `Alt + Shift + v`  | 開啟系統設定    | `gnome-control-center sound`                    |


| 按鍵組合           | 功能                  | 執行指令                     |
| ------------------ | --------------------- | ---------------------------- |
| `Alt + Shift + s`  | 開啟系統設定          | `gnome-control-center`     |
| `Alt + Ctrl + s`   | 開啟擴充模組設定  | `gnome-extensions-app`      |
| `Win + Shift + s`  | 開啟顯示器設定    | `gnome-control-center display`             |
| `Win + Ctrl + s`   | 開啟外觀設定          | `gnome-control-center background`  |


| 按鍵組合      | 功能                | 執行指令                            |
| ------------- | ------------------- | ----------------------------------- |
| `Ctrl + Esc`  | 開啟程序管理器      | `gnome-system-monitor`                 |
| `Win + p`     | 顯示器切換  | `switch-monitor`  |

> `org.gnome.mutter.keybindings switch-monitor`




## 視窗操作

> `org.gnome.desktop.wm.keybindings`

| 按鍵組合       | 功能                               | 設定項目               |
| -------------- | ---------------------------------- | ---------------------- |
| `Alt + Space`  | 顯示「視窗功能選單」               | `activate-window-menu`       |
| `Win + q`      | 關閉視窗                           | `close`     |
| `Win + f`      | 視窗全螢幕                         | `fullscreen_key`       |
| `Win + w`      | 視窗最大化                         | `toggle-fullscreen`  |
| `Win + x`      | 視窗最小化                         | `minimize`      |
| `Win + d`      | 切換「顯示桌面」                   | `show-desktop`     |
| `Win + e`      | 開始「視窗移動」                   | `begin-move`      |
| `Win + r`      | 開始「視窗更改大小」               | `begin-resize`    |
| `Win + t`      | 視窗保持永遠在最上方               | `always-on-top`            |

> 一般預設「`Alt + F4`」綁定「`視窗關閉`」

> 一般預設「`F11`」綁定「`視窗全螢幕`」

> `gsettings list-recursively | grep keybind`

> 也可以在「桌面」，使用「`Win + [滑鼠左鍵拖曳]`」來「移動視窗」

> 也可以在「桌面」，使用「`Win + [滑鼠右鍵拖曳]`」來「更改視窗大小」




## 切換

## 切換 / 視窗

| 按鍵組合     | 功能                        | 設定項目                     |
| ------------ | --------------------------- | ---------------------------- |
| `Win + a`    | 聚焦切換到「前面一個視窗」  | `switch-windows-backward`  |
| `Win + s`    | 聚焦切換到「後面一個視窗」  | `switch-windows`          |


> 一般預設「`Alt + Tab`」綁定「`視窗聚焦切換`」




## 切換 / 工作空間

> `org.gnome.desktop.wm.keybindings`

| 按鍵組合   | 功能                      | 設定項目              |
| ---------- | ------------------------- | --------------------- |
| `Alt + a`  | 切換到「上一個工作空間」  | `switch-to-workspace-left`  |
| `Alt + s`  | 切換到「下一個工作空間」  | `switch-to-workspace-right`  |

> 也可以在「桌面」，使用「`Win + [滑鼠中鍵滾動]`」來「切換工作空間」




## 切換 / 概覽

> `org.gnome.shell.keybindings`

| 按鍵組合       | 功能                        | 設定項目     |
| -------------- | --------------------------- | ------------ |
| `Win + grave`  | 切換到「所有工作空間概覽 / 應用程式啟動選單」  | `toggle-application-view`  |
| `Win + Tab`    | 切換到「所有視窗概覽 / 工作空間概覽」      | `toggle-overview`    |

> 關於「grave」指是「`」，在「Tab鍵」上方的那個「鍵盤按鍵」。




## 其他

> `org.gnome.shell.keybindings`

| 按鍵組合       | 功能                        | 設定項目     |
| -------------- | --------------------------- | ------------ |
| `Win + m`  | 切換顯示「快速設定面板」  | `toggle-quick-settings`  |
| `Win + n`  | 切換顯示「通知訊息歷史列表 / 日曆 面板」  | `toggle-message-tray`  |
| `Win + v`  | 切換到「剪貼簿」  |  |




## 螢幕截圖

> `org.gnome.shell.keybindings`

| 按鍵組合       | 功能                        | 設定項目     |
| -------------- | --------------------------- | ------------ |
| `Print`  | 螢幕截圖  | `screenshot`  |
| `Win + Print`  | 目前聚焦的視窗截圖  | `screenshot-window`  |
| `Alt + Print`  | 截圖面板  | `show-screenshot-ui`  |
| `Win + Control + v`  | 螢幕錄影面板  | `show-screen-recording-ui`  |




## 相關連結

| 相關連結 |
| ------- |
| [鍵盤按鍵綁定](https://samwhelp.github.io/note-about-anduinos-gnome-shell/read/config/keybind.html) |




## 相關專案

| [hotkey-tips](https://github.com/samwhelp/anduinos-gnome-shell-adjustment/tree/main/project/gen/hotkey-tips) |
| ----------- |
| [hotkey-tips.md](https://github.com/samwhelp/anduinos-gnome-shell-adjustment/blob/main/project/gen/hotkey-tips/dist/locale/zh_TW/hotkey-tips.md) |
| [hotkey-tips.tsv](https://github.com/samwhelp/anduinos-gnome-shell-adjustment/blob/main/project/gen/hotkey-tips/dist/locale/zh_TW/hotkey-tips.tsv) |
| [hotkey-tips.sh](https://github.com/samwhelp/anduinos-gnome-shell-adjustment/blob/main/project/gen/hotkey-tips/dist/locale/zh_TW/hotkey-tips.sh) |
