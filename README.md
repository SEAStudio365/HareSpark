<div align="center">

# HareSpark

**Switch apps with a swipe.**

A menu-bar app switcher for macOS, driven entirely by the trackpad.

[**Download the latest release**](../../releases/latest) · [Changelog](CHANGELOG.md) · [繁體中文說明](README.zh-Hant.md)

</div>

---

## What it is

HareSpark lives in your menu bar and turns a trackpad swipe into an app switcher.
Rest your fingers on the trackpad, swipe, and land on the app you want — no
Command-Tab, no reaching for the Dock.

## What makes it different

Click an app's Dock icon and *every* window it owns comes forward, burying
whatever you were looking at. HareSpark goes one level deeper: swipe up on an app
to see its windows, pick one, and **only that window is raised**. The rest stay
exactly where they were.

## The gesture, end to end

| Gesture | What happens |
| :--- | :--- |
| Rest your fingers, then swipe | The switcher opens |
| Swipe left / right | Move through your recent apps |
| Swipe up on an app marked `^` | Open that app's windows |
| Swipe up again | Open the selected window |
| Swipe down, in the window layer | Back to the app list |
| Swipe down, in the app list | Close the switcher, changing nothing |
| Lift off in the window layer | The panel stays put — click a card, or press Esc |

Three fingers to start it (four is also an option). Once the switcher is open,
one, two, or three fingers all steer just as well.

## Requirements

- macOS 13.4 or later
- An Apple trackpad — built-in or a Magic Trackpad
- **Accessibility** permission — required, this is how HareSpark reads gestures
- **Screen Recording** permission — optional, adds a thumbnail of each window.
  Without it everything still works; windows just show as icons.

## Install

1. Download the `.dmg` from [Releases](../../releases/latest)
2. Drag HareSpark into your Applications folder
3. Launch it — a setup guide walks you through permissions and the trackpad
   conflicts described below

Builds are signed with an Apple Developer ID certificate and notarized by Apple.

## Freeing up the trackpad gesture

macOS claims the same swipes for its own gestures, and it sees them before
HareSpark ever does. The setup guide detects exactly which ones clash and links
straight to the right settings pane. The short version:

> System Settings → Trackpad → **More Gestures**, then move **Mission Control**,
> **App Exposé**, and **Swipe between pages / full-screen applications** off the
> finger count HareSpark uses.

The recommended split is HareSpark on three fingers and the system gestures on
four.

If you use three-finger drag, the trigger is locked to *hold, then swipe*, so a
quick three-finger swipe still drags windows the way it always did.

## Settings

- **Gesture** — three or four fingers, swipe or hold-then-swipe, hold time,
  cycling speed
- **Window picker** — icons or cards, preview size
- **Appearance** — system material or frosted glass with adjustable transparency
- **General** — skip apps with no windows, wrap around at the ends, launch at
  login, show or hide the Dock icon
- **Language** — System, English, or 繁體中文

## Pricing

A 7-day trial with everything unlocked. After that:

- **Free, forever** — app switching keeps working
- **Pro** — window previews and sticky mode

One-time payment, no subscription. Buy a coffee at
[buymeacoffee.com/coolfish52](https://buymeacoffee.com/coolfish52), email the
receipt to the address below, and a key comes back. One key covers a limited
number of Macs; you can activate and release them yourself under
Settings → License.

## Updates

HareSpark updates itself. It checks in the background and can install new
versions automatically, or you can check by hand from the menu bar or Settings.

## Privacy

Trackpad input is read on your Mac and never leaves it. The only network requests
HareSpark makes are the update check and, once per Mac, license activation. The
machine code shown in Settings is computed locally and displayed only there.

## Support

Questions, bugs, or licence trouble: **seastudio365@proton.me**

---

<sub>This repository hosts HareSpark's releases and its update feed. The app's
source code is not public.</sub>

<sub>© 2026 SEAStudio365. All rights reserved.</sub>
