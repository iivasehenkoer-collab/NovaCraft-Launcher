# NovaWin 10 Lite

**Version: 1.0.2**  
Target machine: Intel Core i7-9750H · NVIDIA GTX 1650 · 16 GB RAM · Windows x64.

This branch contains the NovaWin 10 Lite ISO builder. It creates installation media locally from an original Microsoft Windows 10 ISO; Windows installation files are not redistributed here.

## Download

[**NovaWin10Lite_1.0.2_Source.zip**](./NovaWin10Lite_1.0.2_Source.zip)

The 1.0.2 release fixes Windows PowerShell 5.1 parsing by saving the ISO builder as UTF-8 with BOM and using ASCII-only diagnostic strings. It also keeps the OEM setup scripts in the installation media root so Windows Setup can copy them into `C:\Windows\Setup\Scripts`.

## Build requirements

- Original Microsoft Windows 10 22H2 x64 ISO
- Windows ADK with **Deployment Tools** (`oscdimg.exe`)
- Administrator PowerShell
- At least 25 GB free disk space recommended

Run `Start-Build.cmd` as administrator, then enter the path to the Microsoft ISO. Output: `NovaWin10Lite_x64.iso`.

## First-logon setup

After Windows is installed and the first local administrator signs in, the package attempts to install Firefox, Steam, Telegram Desktop and WinRAR using WinGet, then downloads and visibly launches the Sota VPN installer. Firefox must be selected manually as the default browser in Windows Settings. Defender, Windows Update and Firewall are retained.

This is not a fully unattended Windows deployment: disk selection, account creation and activation remain part of Windows Setup. Test the ISO in a virtual machine before using it on real hardware.

Windows 10 standard support ended on 14 October 2025. Check Microsoft's ESU availability and eligibility for your device and region.
