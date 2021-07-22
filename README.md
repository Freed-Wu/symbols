# my-x11-keymaps
A backup for the config file of my computer.

<https://github.com/Freed-Wu/my-x11-keymaps/compare/v0.1.0...v0.2.0>

## Usage ##

<pc>: Swap <kbd>Capslock</kbd> and <kbd>Ctrl_R</kbd> in X11.
<altwin>: Change <kbd>Alt_R</kbd> to <kbd>Esc</kbd> in X11.

**NOTE:** Only work in X11 or Wayland.
NOT console.

See [Freed-Wu/my-keymaps](http://www.github.com/Freed-Wu/my-keymaps) to
know keymaps in console.

See [dual-key-remap](https://github.com/ililim/dual-key-remap) and
[xkeymacs](https://github.com/fujieda/xkeymacs) to know keymaps in Window OS.

## Install ##

```
cd /usr/share/X11/xkb/symbols
sudo chown $USER:$USER .
git clone git@github.com:Freed-Wu/my-keymaps
mv my-keymaps/.git* .
git reset --hard
```
