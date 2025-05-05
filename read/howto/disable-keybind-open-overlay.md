---
title: 停用按鍵綁定「Super_L」開啟「Overlay」
nav_order: 7022
has_children: false
parent: 如何
---


# 停用按鍵綁定「Super_L」開啟「Overlay」


## 主題

* [設定指令](#設定指令)
* [恢復指令](#恢復指令)
* [相關議題](#相關議題)
* [備註](#備註)




## 設定指令

執行下面指令，停用按鍵綁定「Super_L」開啟「Overlay」

``` sh
gsettings set org.gnome.mutter overlay-key ''
```




## 恢復指令

若要恢復原本的設定，則是可以執行下面的指令

``` sh
gsettings reset org.gnome.mutter overlay-key
```

或是執行下面的指令，恢復原本的設定

``` sh
gsettings set org.gnome.mutter overlay-key 'Super_L'
```

執行下面的指令，則是觀看目前的設定值

``` sh
gsettings get org.gnome.mutter overlay-key
```

顯示

```
'Super_L'
```




## 相關議題

| 相關議題 |
| ------- |
| [設定「Mouse Button Modifier」](https://samwhelp.github.io/note-about-anduinos-gnome-shell/read/howto/config-mouse-button-modifier.html) |




## gschema

| gschema |
| ------- |
| /usr/share/glib-2.0/schemas/org.gnome.mutter.gschema.xml |


執行下面指令

``` sh
grep 'overlay-key' /usr/share/glib-2.0/schemas/org.gnome.mutter.gschema.xml -A 12
```

顯示

``` xml
    <key name="overlay-key" type="s">
      <default>'Super_L'</default>
      <summary>Modifier to use for extended window management operations</summary>
      <description>
        This key will initiate the “overlay”, which is a combination window
        overview and application launching system.  The default is intended
        to be the “Windows key” on PC hardware.

        It’s expected that this binding either the default or set to
        the empty string.
      </description>
    </key>
```




## 備註

另外在「AnduinOS」內建有安裝「[Arc Menu](https://gitlab.com/arcmenu/ArcMenu)」這個「Gnome Shell 擴充模組」，

> 所以可以執行下面指令，設定「`Alt + F1`」來切換顯示「Arc Menu」。

``` sh

## 處理衝突綁定，先將下面這兩個設定清空。

gsettings set org.gnome.desktop.wm.keybindings panel-main-menu "[]"

gsettings set org.gnome.shell.extensions.apps-menu apps-menu-toggle-menu "[]"

## 設定「`Alt + F1`」來切換顯示「Arc Menu」。

dconf write /org/gnome/shell/extensions/arcmenu/arcmenu-hotkey "['<Alt>F1']"

```

> 可以參考[完整的設定腳本](https://github.com/samwhelp/note-about-anduinos-gnome-shell/blob/gh-pages/_demo/scripts/gnome-shell-keybind/gnome-shell-keybind.sh#L64-L75)
