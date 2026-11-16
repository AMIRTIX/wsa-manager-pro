# WSA Manager Pro

<p align="center">
  <img src="icon.ico" alt="WSA Manager Pro" width="104">
</p>

<h1 align="center">WSA Manager Pro</h1>

<p align="center">
  <strong>Manage your Android apps on Windows — from one simple desktop interface.</strong>
</p>

<p align="center">
  <a href="https://github.com/AMIRTIX/wsa-manager-pro/releases"><img alt="GitHub Releases" src="https://img.shields.io/github/v/release/AMIRTIX/wsa-manager-pro?style=for-the-badge&color=2563eb"></a>
  <a href="https://github.com/AMIRTIX/wsa-manager-pro/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/badge/license-not%20specified-lightgrey?style=for-the-badge"></a>
  <a href="https://github.com/AMIRTIX/wsa-manager-pro"><img alt="Platform" src="https://img.shields.io/badge/platform-Windows-0078D4?style=for-the-badge&logo=windows"></a>
</p>

<p align="center">
  <a href="https://github.com/AMIRTIX/wsa-manager-pro/raw/refs/heads/main/installer/WSA-Manager-Pro-Setup.exe"><strong>⬇ Download for Windows</strong></a>
  &nbsp;·&nbsp;
  <a href="#features">Explore features</a>
  &nbsp;·&nbsp;
  <a href="#getting-started">Get started</a>
</p>

---

## Overview

**WSA Manager Pro** gives you a straightforward graphical way to manage Android applications inside an existing **Windows Subsystem for Android (WSA)** environment.

Connect to WSA, browse installed apps, install supported packages, launch or stop apps, and uninstall applications — without having to manage every task manually.

> **Important:** WSA Manager Pro is a management utility, not an Android emulator. You must install WSA and ADB separately before using the application. It does not install, replace, or provide either of them.

## WSA at a glance

The images below show examples of the Windows Subsystem for Android environment. They are **reference images of WSA, not screenshots of the WSA Manager Pro interface**.

<p align="center">
  <img src="https://cdn.mos.cms.futurecdn.net/9EkX3fVj8kQF9PoekvCkuU-1200-80.jpg" alt="Windows Subsystem for Android settings in dark mode" width="82%">
</p>
<p align="center"><sub>WSA settings in dark mode · <a href="https://www.techradar.com/how-to/how-to-use-windows-subsystem-for-android-in-windows-11">Image source: TechRadar</a></sub></p>

<table>
  <tr>
    <td width="50%">
      <a href="https://cmas.dev/en/posts/2022-04-20-install-android-apps-from-apk/">
        <img src="https://cmas.dev/img/posts/2022/04/20/adb1.png" alt="WSA settings with developer mode" width="100%">
      </a>
      <p align="center"><sub>WSA developer settings · Image source: Christian Amado</sub></p>
    </td>
    <td width="50%">
      <a href="https://www.neowin.net/news/microsoft-publishes-developer-guidance-for-windows-subsystem-for-android/">
        <img src="https://cdn.neowin.com/news/images/uploaded/2021/10/1634737628_fcju5wnx0aqk7h3.jpg" alt="Windows Subsystem for Android settings overview" width="100%">
      </a>
      <p align="center"><sub>WSA settings overview · Image source: Neowin</sub></p>
    </td>
  </tr>
</table>

## Download

<p align="center">
  <a href="https://github.com/AMIRTIX/wsa-manager-pro/raw/refs/heads/main/installer/WSA-Manager-Pro-Setup.exe">
    <img src="https://img.shields.io/badge/Download-WSA_Manager_Pro_Setup-2563EB?style=for-the-badge&logo=windows&logoColor=white" alt="Download WSA Manager Pro Setup">
  </a>
</p>

Download the installer: **[WSA-Manager-Pro-Setup.exe](https://github.com/AMIRTIX/wsa-manager-pro/raw/refs/heads/main/installer/WSA-Manager-Pro-Setup.exe)**

## Features

| Feature | What it does |
| --- | --- |
| **Automatic WSA Connection** | Attempts to start WSA and connect to it. |
| **Application List** | Displays installed third-party Android applications. |
| **APK Installation** | Installs APK files through the connected WSA environment. |
| **App Launching** | Launches installed applications. |
| **App Control** | Stops selected applications. |
| **Uninstallation** | Removes applications after user confirmation. |
| **Search** | Filters apps by name or package identifier. |
| **Activity Log** | Shows operation status and useful feedback. |
| **XAPK / APKS Support** | Basic support, depending on package structure. |
| **Support Window** | Displays project support addresses with copy functionality. |

## Requirements

Before launching WSA Manager Pro, make sure you have:

1. **Windows:** A compatible Windows system.
2. **WSA:** An installed and working version of Windows Subsystem for Android. The official Microsoft version and modified/custom WSA builds are both supported, provided the build works on your Windows system and allows ADB connections.
3. **ADB:** Android Debug Bridge must be installed and accessible on your system.
4. **Developer access:** WSA developer mode / ADB debugging must be enabled when required by your WSA build.

**Important:** WSA Manager Pro does not include or install WSA or ADB. Install and configure both before using the app. Compatibility can vary between WSA builds.

**WSA availability notice:** Microsoft ended general availability of Windows Subsystem for Android through the Microsoft Store on March 5, 2025. Users can use an existing official installation or a compatible modified/custom WSA build.

## Getting Started

1. Install a working WSA build (official Microsoft or modified/custom).
2. Install ADB and make sure it is accessible on your system.
3. Enable WSA developer mode / ADB debugging if your build requires it.
4. Download and run the WSA Manager Pro installer.
5. Launch **WSA Manager Pro**.
6. Select **Auto Setup WSA**.
7. Wait for the connection status to update.
8. Refresh the application list if necessary.

## Managing Applications

### Install an APK

1. Select **Install App**.
2. Choose an APK file.
3. Wait for the installation to finish.
4. Check the activity log for the result.

### Launch, stop, or uninstall

Select an installed application and use its **Launch**, **Stop**, or **Uninstall** action. Uninstallation requires confirmation.

### Search applications

Enter an application name or package identifier in the search field.

## Supported Package Formats

| Format | Support |
| --- | --- |
| APK | Standard installation |
| XAPK | Basic archive-based installation |
| APKS | Basic split-package installation |

Some application bundles require additional split APK selection, OBB files, or package-specific installation steps. These cases may not be supported.

## Troubleshooting

| Problem | Suggested action |
| --- | --- |
| WSA connection fails | Verify that WSA is installed, running, and has ADB debugging enabled. |
| ADB is not detected | Install ADB and make sure it is accessible on your system. |
| No applications appear | Check the WSA/ADB connection, then refresh the application list. |
| APK installation fails | Check the package file, ADB connection, and WSA status. |
| An application does not launch | Verify that it is installed and compatible with your WSA build. |
| XAPK/APKS installation fails | The package may require split APK or OBB handling that is not supported. |

## Limitations

- WSA Manager Pro does not install or replace WSA or ADB.
- It does not automatically enable WSA developer settings.
- Some Android application bundles may require installation steps beyond the supported functionality.
- Compatibility depends on the Windows and WSA environment, including the specific WSA build.
- Not every Android application is guaranteed to work under WSA.

## Support the Project

If you find WSA Manager Pro useful, you can support the project through the addresses shown in the application's **Support This App** window.

The application only displays and copies these addresses. It does not connect to wallets or process payments.

## Disclaimer

WSA Manager Pro is an independent community project. It is not affiliated with, endorsed by, or supported by Microsoft.

Windows Subsystem for Android, Android, and ADB are products or trademarks of their respective owners.

Use the application at your own discretion. Always review application packages before installing them.

## License

No open-source license has been specified. All rights and permissions remain subject to the copyright holder's terms until a license is added.

---

<p align="center">
  <strong>WSA Manager Pro</strong><br>
  <em>A simpler way to manage Android apps on Windows.</em>
</p>
