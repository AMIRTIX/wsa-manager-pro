# WSA Manager Pro

<p align="center">
  <strong>A simple desktop application for managing Android apps on Windows Subsystem for Android.</strong>
</p>

<p align="center">
  <img src="icon.ico" alt="WSA Manager Pro icon" width="96">
</p>

---

## Overview

**WSA Manager Pro** provides a convenient graphical interface for managing Android applications in an existing Windows Subsystem for Android (WSA) environment.

Connect to WSA, browse installed apps, install supported Android packages, launch or stop applications, and uninstall apps when they are no longer needed.

> **Important:** WSA Manager Pro is not an Android emulator and does not install or replace WSA. A working WSA environment is required.

## Download

Get the Windows installer:

**[Download WSA Manager Pro Setup](https://github.com/AMIRTIX/wsa-manager-pro/raw/refs/heads/main/installer/WSA-Manager-Pro-Setup.exe)**

The installer will be available at this link once the setup file has been uploaded to the repository.

## Features

- **Automatic WSA Connection** — Attempts to start WSA and connect to it.
- **Application List** — Displays installed third-party Android applications.
- **APK Installation** — Installs APK files through the connected WSA environment.
- **App Launching** — Launches installed applications.
- **App Control** — Stops selected applications.
- **Uninstallation** — Removes applications after user confirmation.
- **Search** — Filters apps by name or package identifier.
- **Activity Log** — Shows operation status and useful feedback.
- **XAPK / APKS Support** — Basic support, depending on package structure.
- **Support Window** — Displays project support addresses with copy functionality.

## Requirements

- A compatible Windows system.
- An existing and functional WSA installation.
- Android Debug Bridge (ADB) available to the application.
- WSA developer settings configured when required.

**WSA availability notice:** Microsoft ended the general availability of Windows Subsystem for Android through the Microsoft Store in 2025. This application is intended for users who already have a working WSA installation.

## Installation

1. Download **WSA-Manager-Pro-Setup.exe** using the link above.
2. Run the installer.
3. Follow the installation instructions.
4. Launch **WSA Manager Pro** from the installed application or shortcut.

## Getting Started

1. Make sure WSA is installed and available on your system.
2. Open WSA Manager Pro.
3. Select **Auto Setup WSA**.
4. Wait for the connection status to update.
5. Refresh the application list if necessary.
6. Select an application to manage it.

## Managing Applications

### Install an APK

1. Select **Install App**.
2. Choose an APK file.
3. Wait for the installation to finish.
4. Check the activity log for the result.

### Launch an Application

Select an installed application and use its **Launch** action.

### Stop an Application

Use the **Stop** action to stop the selected Android application.

### Uninstall an Application

Use the **Uninstall** action and confirm the operation.

### Search Applications

Enter an application name or package identifier in the search field.

## WSA Connection

### Auto Setup WSA

This option attempts to start WSA, establish an ADB connection, and load the installed application list.

### Disconnect & Close WSA

This option attempts to disconnect ADB and close relevant WSA processes.

Connection and shutdown results depend on the local WSA environment.

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
| WSA connection fails | Verify that WSA is installed and running correctly. |
| ADB is not detected | Make sure ADB is available to the application. |
| No applications appear | Check the WSA connection, then refresh the application list. |
| APK installation fails | Check the package file and the WSA connection. |
| An application does not launch | Verify that it is installed and compatible with WSA. |
| XAPK/APKS installation fails | The package may require split APK or OBB handling that is not supported. |

## Limitations

- WSA Manager Pro does not install or replace WSA.
- It does not automatically enable WSA developer settings.
- Some Android application bundles may require installation steps beyond the supported functionality.
- Compatibility depends on the Windows and WSA environment.
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
