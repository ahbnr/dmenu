A copy of the [dmenu](https://tools.suckless.org/dmenu/) dynamic menu for X
repository including my configuration and patches I use.

Running `build.sh` resets the repository, applies the patches and builds dmenu.

Build an install an Arch Linux package like this:
```sh
makepkg -sif PKGBUILD
```

Used patches:

* [border](https://tools.suckless.org/dmenu/patches/border/)
* [center](https://tools.suckless.org/dmenu/patches/center/)

Configuration changes:

* border width of 4
