<div align="center">

# React Native Dev Paradise

**Run your React Native projects without a terminal.**

Every command, device, log and network request for every project — in one place,
so you can stop juggling terminal tabs.

[![Download](https://img.shields.io/badge/Download-latest%20release-4f9dff?style=for-the-badge)](../../releases/latest)
![macOS](https://img.shields.io/badge/macOS-Intel%20%26%20Apple%20silicon-black?style=flat-square&logo=apple)
![Windows](https://img.shields.io/badge/Windows-10%20%26%2011-0078D6?style=flat-square&logo=windows)
![Linux](https://img.shields.io/badge/Linux-deb%20%26%20tar.gz-F0A81B?style=flat-square&logo=linux)

<img alt="React Native Dev Paradise — projects, commands and logs in one window" width="900" src="https://github.com/user-attachments/assets/8edec80f-4eea-4110-862d-c7e762f843ba" />

</div>

---

## What it does

| | |
|---|---|
| **Run anything** | Metro, a build, a test run — as many at once as you like, each with its own live output. Stopping one takes its whole process tree with it. |
| **It reads your project** | Open a folder and it tells you what the checkout already describes: `package.json` scripts, Makefile targets, fastlane lanes. Near-identical commands are folded into one card with variants — debug, staging, release — instead of five. |
| **One command, many lines** | Keep several command lines behind one card and switch between them without editing anything. |
| **Devices on tap** | Boot and shut down simulators and emulators from the sidebar, and see at a glance what is running. |
| **Logs that make sense** | Your app's `console.log` next to Metro's output, and the device's own native log per simulator or emulator. Search and filter without losing a line — matches are hidden, never discarded. |
| **See network requests** | Every request the running app makes, grouped by device, with headers and bodies. No proxy to set up, no extra dependency. |
| **Knows your machine** | Checks Node, a package manager, the JDK, the Android SDK, adb, Xcode and CocoaPods, and offers to install what is missing. |
| **Four languages** | English, Português (BR), Norsk and Español. |

## Install

Grab the file for your system from the **[latest release](../../releases/latest)** and double-click it.

| System | File | Notes |
|---|---|---|
| **macOS** | `…-macos.pkg` | Intel and Apple silicon, one build for both. See the note below. |
| **Windows** | `…-windows.zip` | Unzip, then run **`Install React Native Dev Paradise.cmd`**. |
| **Linux** | `…_all.deb` | Debian, Ubuntu, Mint, Pop!_OS — double-click and the desktop's installer takes over. |
| **Linux** | `…-linux.tar.gz` | Everything else. Unpack and run `./install.sh` — installs for you only, no root needed. |

**Node.js 20 or newer** is the one thing it needs. If you have not got it, the installer says so and offers to
install it for you rather than failing quietly.

### macOS: "Apple could not verify…"

macOS blocks any download that is not signed with a paid Apple Developer ID, and says so in alarming
words. Nothing is wrong with the app — macOS simply cannot tell who built it. It takes one answer, once.

**Either** open the file, dismiss the warning, then go to  **System Settings → Privacy & Security**,
scroll down to **Security**, and press **Open Anyway** next to the app's name.

**Or** run this first, then open the file normally:

```sh
xattr -dr com.apple.quarantine ~/Downloads/react-native-dev-paradise-*-macos.*
```

> Guides that tell you to **right-click → Open** are out of date: macOS 15 removed that shortcut.

> The app runs entirely on your own machine. It opens in your browser at `127.0.0.1` and talks to nothing
> else — no account, no telemetry, no cloud.

## Updating

The app checks this repository for new releases and can install them for itself: **Settings › Updates**,
where you can also turn on automatic updates. Your projects, commands, groups and settings are stored
outside the app and are never touched by an update.

## Uninstalling

| System | |
|---|---|
| macOS | Drag the app from **Applications** to the Bin. |
| Windows | Run `uninstall.cmd` from the install folder. |
| Linux | `sudo apt remove react-native-dev-paradise`, or `./uninstall.sh` for the tarball. |

Your settings live in `~/.react-native-dev-paradise` and are left alone, so reinstalling picks up where
you left off. Delete that folder if you want a clean slate.

<div align="center">

---

Made by [edu90k](https://github.com/eduardo-santos)

</div>

