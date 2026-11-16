# WSA Manager Pro

<p align="center">
  <strong>A desktop utility for managing Android applications on Windows Subsystem for Android (WSA).</strong>
</p>

<p align="center">
  <img src="icon.ico" alt="WSA Manager Pro icon" width="96">
</p>

<p align="center">
  <strong>Windows Desktop Application · Python · CustomTkinter · ADB</strong>
</p>

---

## Overview

**WSA Manager Pro** is a Windows desktop application designed to simplify the management of Android applications running through Windows Subsystem for Android (WSA).

It provides a graphical interface for connecting to WSA, browsing installed Android applications, installing APK packages, launching and stopping apps, and uninstalling applications.

The application uses Android Debug Bridge (ADB) to communicate with an existing WSA installation.

> **Important:** WSA Manager Pro is a management utility, not an Android emulator or a replacement for WSA. It does not install WSA or enable Android developer settings automatically.

## Features

- **Automatic WSA Connection** — Attempts to start WSA and establish an ADB connection.
- **Application Management** — Lists installed third-party Android applications.
- **APK Installation** — Installs APK files through ADB.
- **App Launching** — Starts installed Android applications.
- **App Control** — Stops applications using Android package commands.
- **Application Uninstallation** — Removes applications after user confirmation.
- **Search** — Filters applications by name or package identifier.
- **Activity Log** — Displays timestamped application events and operation results.
- **XAPK / APKS Support** — Provides basic package installation support, subject to package structure and split APK limitations.
- **Donation Window** — Displays supported cryptocurrency addresses with copy functionality.

## Interface

The application uses a dark desktop interface with two main areas:

| Section | Description |
| --- | --- |
| Sidebar | WSA connection controls, connection status, refresh, log clearing and support |
| Main panel | Android application management, APK installation, search and activity log |

## Requirements

Before using WSA Manager Pro, make sure you have:

- A compatible Windows installation.
- An existing and functional WSA installation.
- Android Debug Bridge (ADB).
- WSA developer settings configured when required.
- Android application packages in a supported format.

**WSA availability notice:** Microsoft ended the general availability of Windows Subsystem for Android through the Microsoft Store in 2025. This project is intended for users who already have a working WSA installation.

## Getting Started

1. Download and install WSA Manager Pro.
2. Make sure WSA is installed and available on your system.
3. Open WSA Manager Pro.
4. Select **Auto Setup WSA**.
5. Wait for the connection status to update.
6. Refresh the application list if necessary.
7. Select an application to manage it.

## Application Management

### Install an APK

1. Select **Install App**.
2. Choose an APK file.
3. Wait for ADB to complete the installation.
4. Check the activity log for the result.

### Launch an Application

Select an installed application and use its **Launch** action.

### Stop an Application

Use the **Stop** action to force-stop the selected Android package.

### Uninstall an Application

Use the **Uninstall** action and confirm the operation.

### Search Applications

Enter an application name or package identifier in the search field.

## WSA Connection

### Auto Setup WSA

The automatic connection process attempts to:

- Start WSA.
- Connect to the default ADB endpoint.
- Retry the connection when necessary.
- Update the connection status.
- Load installed applications after a successful connection.

### Disconnect & Close WSA

This action attempts to disconnect ADB and close relevant WSA processes.

**Note:** Connection and shutdown results depend on the local WSA and ADB environment.

## Supported Package Formats

| Format | Support |
| --- | --- |
| APK | Standard installation through ADB |
| XAPK | Basic archive-based installation |
| APKS | Basic split-package installation |

Some application bundles require additional split APK selection, OBB files, or package-specific installation steps. These cases may not be supported by the current implementation.

## Activity Log

The activity log provides feedback about operations performed by the application.

Log categories include:

- Info
- Success
- Warning
- Error

Use **Clear Log** to clear the visible activity history.

## Troubleshooting

| Problem | Suggested action |
| --- | --- |
| WSA connection fails | Verify that WSA is installed and running correctly. |
| ADB is not detected | Install ADB or make sure its executable is accessible through PATH. |
| No applications appear | Confirm that ADB is connected to the correct WSA instance, then refresh the list. |
| APK installation fails | Check the APK file and the ADB connection. |
| An application does not launch | Verify that the application is installed and compatible with the WSA environment. |
| XAPK/APKS installation fails | The package may require split APK or OBB handling not supported by the current implementation. |

## Technology Stack

- **Python** — Application logic.
- **CustomTkinter** — Desktop graphical interface.
- **ADB** — Android device communication.
- **Subprocess** — External process management.
- **Threading** — Background operations.
- **ThreadPoolExecutor** — Concurrent task execution.
- **PyInstaller** — Windows executable packaging.
- **Inno Setup** — Windows installer generation.

## Project Structure

```text
WSA-Manager-Pro/
│
├── test.py
├── icon.ico
├── README.md
├── requirements.txt
├── .gitignore
│
├── installer/
│   └── WSA-Manager-Pro-Setup.exe
│
└── dist/
    └── WSA Manager Pro/
        └── WSA Manager Pro.exe
```

*The actual repository structure may differ depending on the final build and release files.*

## Building from Source

### 1. Clone the repository

```bash
git clone https://github.com/AMIRTIX/wsa-manager-pro.git
cd wsa-manager-pro
```

### 2. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 3. Run the application

```bash
python test.py
```

### 4. Build the executable

The project uses PyInstaller for packaging.

```bash
pyinstaller --noconfirm --windowed --name "WSA Manager Pro" --icon icon.ico test.py
```

The generated executable is placed in the `dist` directory.

### 5. Build the Windows installer

The Windows installer is generated separately using Inno Setup and the project's installer configuration.

The installer should be tested on a clean Windows environment before release.

## Limitations

- WSA Manager Pro does not install or replace WSA.
- It does not automatically enable WSA developer settings.
- ADB must be available to the application.
- Some Android application bundles may require installation procedures beyond the current implementation.
- Compatibility depends on the user's Windows, WSA and ADB environment.
- Not every Android application is guaranteed to work under WSA.

## Support the Project

If you find WSA Manager Pro useful, you can support its development through the addresses provided in the application's **Support This App** window.

The application only displays and copies these addresses. It does not connect to wallets or process payments.

## Disclaimer

WSA Manager Pro is an independent community project. It is not affiliated with, endorsed by, or supported by Microsoft.

Windows Subsystem for Android, Android, and ADB are trademarks or products of their respective owners.

Use the application at your own discretion. Always review package files before installing them.

## License

No open-source license has been specified yet. All rights and permissions remain subject to the copyright holder's terms until a license is added.

---

<p align="center">
  <strong>WSA Manager Pro</strong><br>
  <em>A simpler way to manage Android apps on Windows.</em>
</p>
