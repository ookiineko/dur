dropout user repository (dur)
=============================

yet another binary repo of aur pkgs

currently only x86_64 is supported

## For who

* stock wine gaming mainly Japanese VNs
* software development of multiple stacks
* KDE desktop users

## What's included

so far it mainly has:

* `lib32-` pkgs needed by wine or AOSP build
* non-WoW64 build of a stable pinned ver of wine
* `qt6-wasm`
* Qt Widgets and its dependencies for arch MinGW toolchain
* `wget2`
* `java-language-server-git`
* `koi`
* could be some others that i personally use

> [!NOTE]
> * dur pkgs are updated when i feel upgrading my system
> * pkgs might be added or removed over time
> * pkgs might not be the latest (updated when dependency breaks, or when i figured out i need a newer version)
> * dur patches out some bugs or code of poor quality
> * non-binary pkgs or small pkgs might not be in dur

## What to note

* to use `wine`, install `wine-mono` from https://archive.archlinux.org/packages/w/wine-mono/wine-mono-10.0.0-1-x86_64.pkg.tar.zst and hold it in `pacman.conf`

## FIXME/TODOs

* currently `wine` needs to be manually held in `pacman.conf` and pkgname is still `wine` instead of `wine32`

## Usage

to use dur, add these into your `/etc/pacman.conf`:

```ini
[dur]
SigLevel = Optional
Server = https://random-mirrors.d0ve.workers.dev/0:/dur/
```

## Patched AUR pkgs

(occasional compilation fixes are quick to me and thus not uploaded to github)

| name | PKGBUILD repo url |
| --- | --- |
| `wine` | https://github.com/ookiineko/wine-PKGBUILD |
| `mingw-w64-zstd` | https://github.com/ookiineko/mingw-w64-zstd-PKGBUILD |
| `mingw-w64-brotli` | https://github.com/ookiineko/mingw-w64-brotli-PKGBUILD |
| `mingw-w64-cmake-static` | https://github.com/ookiineko/mingw-w64-cmake-static-PKGBUILD |
