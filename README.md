<p align="center"><img src="./app/assets/images/SealCircle.png" width="150px" height="150px" alt="aventium softworks"></p>

<h1 align="center">Starbounded Launcher</h1>

<em><h5 align="center">(forked from Helios Launcher, formerly Electron Launcher)</h5></em>

[<p align="center"><img src="https://img.shields.io/github/actions/workflow/status/starbounded-dev/starbounded-launcher/build.yml?branch=master&style=for-the-badge" alt="gh actions">](https://github.com/dscalzi/HeliosLauncher/actions) [<img src="https://img.shields.io/github/downloads/starbounded-dev/starbounded-launcher/total.svg?style=for-the-badge" alt="downloads">](https://github.com/dscalzi/HeliosLauncher/releases) <img src="https://forthebadge.com/images/badges/winter-is-coming.svg"  height="28px" alt="winter-is-coming"></p>

<p align="center">Join modded servers without worrying about installing Java, Forge, or other mods. We'll handle that for you.</p>

![Screenshot 1](https://i.imgur.com/mrjpY4X.png)
![Screenshot 2](https://i.imgur.com/qSFn8Bm.png)

## Features

* 🔒 Full account management.
  * Add multiple accounts and easily switch between them.
  * Microsoft (OAuth 2.0) + Mojang (Yggdrasil) authentication fully supported.
  * Credentials are never stored and transmitted directly to Mojang.
* 📂 Efficient asset management.
  * Receive client updates as soon as we release them.
  * Files are validated before launch. Corrupt or incorrect files will be redownloaded.
* ☕ **Automatic Java validation.**
  * If you have an incompatible version of Java installed, we'll install the right one *for you*.
  * You do not need to have Java installed to run the launcher.
* 📰 News feed natively built into the launcher.
* ⚙️ Intuitive settings management, including a Java control panel.
* Supports all of our servers.
  * Switch between server configurations with ease.
  * View the player count of the selected server.
* Automatic updates. That's right, the launcher updates itself.
*  View the status of Mojang's services.

This is not an exhaustive list. Download and install the launcher to gauge all it can do!

#### Like the project? Leave a ⭐ star on the repository!

## Downloads

You can download from [GitHub Releases](https://github.com/dscalzi/HeliosLauncher/releases)

**Supported Platforms**

If you download from the [Releases](https://github.com/dscalzi/HeliosLauncher/releases) tab, select the installer for your system.

| Platform | File                                      |
| -------- |-------------------------------------------|
| Windows x64 | `Starbounded-Launcher-setup-VERSION.exe`  |
| macOS x64 | `Starbounded-Launcher-setup-VERSION-x64.dmg`   |
| macOS arm64 | `Starbounded-Launcher-setup-VERSION-arm64.dmg` |
| Linux x64 | `Starbounded-Launcher-setup-VERSION.AppImage`  |

## Console

To open the console, use the following keybind, just as a chronium browser.

```console
ctrl + shift + i
```

Ensure that you have the console tab selected. Do not paste anything into the console unless you are 100% sure of what it will do. Pasting the wrong thing can expose sensitive information.

#### Export Output to a File

If you want to export the console output, simply right click anywhere on the console and click **Save as..**

![console example](https://i.imgur.com/T5e73jP.png)


## Development

This section details the setup of a basic developmentment environment.

### Getting Started

**System Requirements**

* [Node.js][nodejs] v20

---

**Clone and Install Dependencies**

```console
> git clone https://github.com/starbounded-dev/starbounded-launcher.git
> cd starbounded-launcher
> npm install
```

---

**Launch Application**

```console
> npm start
```

---

**Build Installers**

To build for your current platform.

```console
> npm run dist
```

Build for a specific platform.

| Platform    | Command              |
| ----------- | -------------------- |
| Windows x64 | `npm run dist:win`   |
| macOS       | `npm run dist:mac`   |
| Linux x64   | `npm run dist:linux` |

Builds for macOS may not work on Windows/Linux and vice-versa.

---