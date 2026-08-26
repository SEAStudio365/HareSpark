# Changelog

All notable changes to HareSpark. [繁體中文](CHANGELOG.zh-Hant.md)

## 1.4.3

**Fixed**

- **Finder now opens a new window.** Lifting off on Finder when it has no windows
  open used to focus it and show nothing. It now opens a fresh window, the same
  way clicking the Dock icon does. Finder also stays in the app strip when
  "Skip apps with no windows" is on, since it can always be opened into.
- **No more phantom entries in the window list.** Some apps — Electron ones in
  particular — keep tiny helper windows that carry an ordinary window role.
  Those showed up as unpickable cards with no preview, and closing them did
  nothing because the app rebuilt them immediately. Windows now have to be big
  enough to be real, matching the threshold the app switcher already used.
- **App icons no longer fall back to a folder.** When a bundle carries a stale
  custom-icon flag with no icon behind it, macOS hands back the plain folder
  icon — even though the Dock and Command-Tab still show the real one.
  HareSpark now spots that case and reads the app's own icon instead.

**Internal**

- Update signing keys were rotated. Existing installs update as normal; nothing
  to do on your end.

## 1.4.2 and earlier

See the [Releases page](../../releases).
