---
title: 將「常用的應用程式」固定顯示在下方「Panel」(favorite-apps)
nav_order: 7031
has_children: true
parent: 如何
---


# 將「常用的應用程式」固定顯示在下方「Panel」(favorite-apps)


## 主題

* [前提](#前提)
* [指令設定](#指令設定)
* [備註](#備註)




## 前提

除了可以透過「圖形介面」來「操作」，將「常用的應用程式」固定顯示在下方「Panel」。

也可以透過「[指令](#指令設定)」來設定。




## 指令設定

舉例，執行下面指令

``` sh
gsettings set org.gnome.shell favorite-apps "['org.gnome.Nautilus.desktop', 'org.gnome.TextEditor.desktop', 'firefox.desktop', 'org.gnome.Console.desktop', 'org.gnome.Settings.desktop', 'org.gnome.Software.desktop']"
```


就會將上面「列舉的應用程式」固定顯示在下方「Panel」。

> 另外預設可以透過「`Win + 1~9`」來對應「開啟或聚焦」該應用程式。

也就是

| 按鍵組合           | 對應「開啟或聚焦」應用程式                   |
| ------------------ | ---------------------- |
| `Win + 1`  | 'org.gnome.Nautilus.desktop'                   |
| `Win + 2`  | 'org.gnome.TextEditor.desktop'                   |
| `Win + 3`  | 'firefox.desktop'                   |
| `Win + 4`  | 'org.gnome.Console.desktop'                   |
| `Win + 5`  | 'org.gnome.Settings.desktop'                   |
| `Win + 6`  | 'org.gnome.Software.desktop'                   |




## 備註

執行

``` sh
gsettings list-recursively | grep keybind | grep switch-to-application
```

顯示

```
org.gnome.shell.keybindings switch-to-application-1 ['<Super>1']
org.gnome.shell.keybindings switch-to-application-2 ['<Super>2']
org.gnome.shell.keybindings switch-to-application-3 ['<Super>3']
org.gnome.shell.keybindings switch-to-application-4 ['<Super>4']
org.gnome.shell.keybindings switch-to-application-5 ['<Super>5']
org.gnome.shell.keybindings switch-to-application-6 ['<Super>6']
org.gnome.shell.keybindings switch-to-application-7 ['<Super>7']
org.gnome.shell.keybindings switch-to-application-8 ['<Super>8']
org.gnome.shell.keybindings switch-to-application-9 ['<Super>9']
```
