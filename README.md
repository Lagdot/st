
The [suckless terminal](https://st.suckless.org) with some extra stuff
Based on Luke Smith's build

Made with dmenu in mind

## Bindings

+ **scrollback** with `alt-↑/↓` or `alt-pageup/down` or `shift` while scrolling the mouse.
+ OR **vim-bindings**: scroll up/down in history with `alt-k` and `alt-j`. Faster with `alt-u`/`alt-d`.
+ **zoom/change font size**: same bindings as above, but holding down shift aswell. `alt-home` returns to default
+ **copy text** with `alt-c`, **paste** is `alt-v` or `shift-insert`

## Pretty stuff

+ Compatible with `Xresources` and (kinda) `pywal`
+ Transparency/alpha

## Installation

```
git clone https://Lagdot/st
cd st
doas make install
```

(or use sudo)

Obviously, `make` is required to build. `fontconfig` is required for the
default build, since it asks `fontconfig` for your system monospace font. It
might be obvious, but `libX11` and `libXft` are required as well

On OpenBSD, you'll also need to edit `config.mk` and remove `-lrt` from the `$LIBS` before compiling

Also be sure to have a composite manager like `picom` or `xcompmgr` running if you want transparency to work
