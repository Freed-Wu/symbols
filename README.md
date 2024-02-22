# my-x11-keymaps
A backup for the config file of my computer.

<https://github.com/Freed-Wu/my-x11-keymaps/compare/v0.1.0...v0.2.0>

## Usage ##

<pc>: Swap <kbd>Capslock</kbd> and <kbd>Ctrl_R</kbd> in X11.
<altwin>: Change <kbd>Alt_R</kbd> to <kbd>Esc</kbd> in X11.

**NOTE:** Only work in X11 or Wayland.
NOT console.

## Install ##

```sh
cd /usr/share/X11/xkb/symbols
sudo chown $USER:$USER .
git clone git@github.com:Freed-Wu/my-keymaps
mv my-keymaps/.git* .
git reset --hard
```

## Related Projects ##

- [Freed-Wu/my-keymaps](http://github.com/Freed-Wu/my-keymaps): my keymaps in console
- [Freed-Wu/etc](http://github.com/Freed-Wu/etc): my keymaps in Windows.
- [My keymap in Android](https://github.com/Freed-Wu/symbols/releases/download/v0.1.0/ExKeyMo.Keyboard.Layout.apk)
  Need [exkeymo-web](https://github.com/ris58h/exkeymo-web).
  It swaps:

  - <kbd>capslock</kbd> and <kbd>ctrl</kbd>
  - <kbd>cmd</kbd> and <kbd>alt</kbd>
  - <kbd>esc</kbd> and <kbd>home</kbd>
  - <kbd>power</kbd> and <kbd>delete</kbd>

```sh
# uninstall old
adb uninstall ris58h.exkeymo_keyboard_layout
adb install ExKeyMo.Keyboard.Layout.apk
```

`res/Q2.kcm`:

```kcm
type OVERLAY

# Modifications made by ExKeyMo project:
map key 111 POWER
map key 1 HOME
map key 56 META_LEFT
map key 58 CTRL_RIGHT
map key 125 ALT_LEFT
map key 116 FORWARD_DEL
map key 172 ESCAPE
map key 97 CAPS_LOCK
```
