---
layout: default
title: Autounattend Generator
---

Create a Windows 10/11 `autounattend.xml` answer file by picking options in tabs: installation, user account, privacy, performance, power, updates, theme, taskbar, apps and more. Everything runs in your browser. Nothing is uploaded anywhere.

<p><a class="btn" href="{{ '/generator.html' | relative_url }}">Open the generator</a></p>

## What you can configure

- **Windows setup:** language, keyboard, time zone, edition and product key, Windows 11 hardware-check bypasses, optional automatic disk partitioning, network disabled during setup, OOBE screens.
- **User account:** automatic local account, computer name, one-time auto-logon.
- **Optimize:** privacy and security, performance and gaming, power, updates, notifications and sound.
- **Customize:** theme, taskbar, Start menu, File Explorer.
- **Debloat:** one-click levels (Minimal, Recommended, ULTIMATE) for removing bloatware, with every item adjustable.
- **Apps:** remove built-in Windows apps, optional features and OneDrive.
- **Software:** install programs with winget on first logon.

## How to use

1. Open the generator and choose your options (or start from the *Recommended* or *Gaming* preset).
2. Go to **Generate XML**, read the warnings and download `autounattend.xml`.
3. Copy the file to the root of your Windows installation USB drive, next to `setup.exe`.
4. Boot from the USB drive and install Windows.

> The generator starts in English (US); use the language menu in its top bar to switch language (Portuguese is included).

## Read before using

- The optional automatic partitioning **erases disk 0** without asking. Test in a virtual machine first.
- A password set for the local account is stored **in plain text** inside the XML. Do not share that file.
- This is an independent project, not affiliated with or endorsed by Winhance. It generates a standard answer file with embedded scripts that apply equivalent tweaks.
- Use at your own risk. Always review the generated XML.

[Source code and documentation on GitHub]({{ site.github.repository_url }})
