---
layout:     post
title:      "Xubuntu 23.10 Release Notes"
date:       2023-10-12 02:23:44 +0200
categories: 2310
---
**Welcome to the Xubuntu 23.10 “Mantic Minotaur” release notes!**

Xubuntu 23.10 was released on Thursday, October 12, 2023, and will be supported for nine months until July 2024. For general information and the latest updates for Xubuntu 23.10, check out the [release page on](https://xubuntu.org/release/23-10) xubuntu.org.

* [Known Issues](#known-issues)
* [Ubuntu Common Release Notes](#ubuntu-common-release-notes)
* [Major Updates](#major-updates)
* [Appearance Updates](#appearance-updates)
* [Updates](#updates)
* [Changelogs](#changelogs)

## Known Issues
### Installer Issues

* No shutdown prompt after installation ([1944519](https://launchpad.net/bugs/1944519))
  * However, you should be able to press the Enter key to continue with the reboot.
* Xubuntu installer on desktop is “untrusted” ([1987958](https://launchpad.net/bugs/1987958))
  * The launcher can be run from the menu or you can click “Launch anyway”.
* OEM installation fails on Xubuntu Minimal ([2013251](https://launchpad.net/bugs/2013251))
* Installer crashes when quitting in the live session ([2016009](https://launchpad.net/bugs/2016009))

### General Issues

* **Xfce Pulseaudio Plugin**
  * Multiple notifications displayed if multiple Pulseaudio plugins added to panel ([1769775](https://launchpad.net/bugs/1769775))
* **Virtual Machines**
  * Xorg crashes after logging in or switching users on some virtual machines, including QEMU/GNOME Boxes and Virtualbox ([1861609](https://launchpad.net/bugs/1861609))
  * Poor performance and audio stuttering in some virtual machines, including VMware and VirtualBox
    * In these instances, you will need to either adjust your configuration (recommended) or replace PipeWire with PulseAudio

### Ubuntu Common Release Notes

The main [Ubuntu Release Notes](https://discourse.ubuntu.com/t/mantic-minotaur-release-notes/35534) covers both many of the other packages we carry and more issues common to every Ubuntu flavor.

## Major Updates

* Xfce libraries, including **garcon**, **libxfce4ui**, **tumbler**, and **xfconf** have received several bug fixes for race conditions and memory leaks. Overall, the desktop should be more responsive and less prone to crash.
* **Mousepad 0.6.1** features better modification state tracking, UX improvements, and a new “match whole word” toggle added to the search toolbar.
* **Ristretto 0.13.1** adds printing support to Xubuntu's default image viewer.
* **Xfce Power Manager 4.18.2** and **Xfce Screensaver 4.18.2** received several updates to eliminate screensaver issues.
* **Xfce PulseAudio Plugin 0.4.7** received several bug fixes and updates to its media player and audio device handling. Media players can now be marked as persistent or ignored via the settings dialog.
* **Xfce Screenshooter 1.10.4** added support for AVIF and JPEG XL file formats.
* Numerous additional stable release updates for Xfce 4.18 and related applications.

## Appearance Updates

* **[elementary-xfce](https://github.com/shimmerproject/elementary-xfce/releases/tag/v0.18)** 0.18 features numerous refreshed icons across the entire Xubuntu desktop.
* **[Greybird 3.23.3](https://github.com/shimmerproject/Greybird/releases/tag/v3.23.3)** improves GTK 3 and 4 support.
* Some GNOME components, including **Disk Usage Analyzer** (baobab), **Fonts** (gnome-font-viewer), and **Document Scanner** (simple-scan) have a refreshed interface using libadwaita and newer design conventions.
* Several Xfce components have been updated to better support UI scaling. 2x scaling can be enabled from the Appearance dialog.
* **Color emoji** 😉️ are now included and used in Firefox, Thunderbird, and Gtk 3 and newer applications. To enter emoji on Gtk applications (such as Mousepad), use the `Ctrl + .` keyboard shortcut to show the emoji picker.
* When changing your Gtk (interface) theme, a matching Xfwm (window manager) theme is now automatically selected. This setting can be changed in the Appearance dialog.
* **[Past Xubuntu wallpapers](https://github.com/Xubuntu/xubuntu-marketing/blob/master/wallpapers/README.md)** can now be easily installed from the repositories! They're grouped by LTS release:
  * `xubuntu-wallpapers-jammy`: Hirsute, Impish, and Jammy
  * `xubuntu-wallpapers-focal`: Cosmic, Disco, Eoan, and Focal
  * `xubuntu-wallpapers-bionic`: Yakkety, Zesty, Artful, and Bionic
  * `xubuntu-wallpapers-xenial`: Utopic, Vivid, Wily, and Xenial
  * `xubuntu-wallpapers-trusty`: Quantal, Raring, Saucy, and Trusty
  * `xubuntu-wallpapers-precise`: Maverick, Natty, and Precise
  * `xubuntu-wallpapers-lucid`: Intrepid, Jaunty, Karmic, and Lucid
  * `xubuntu-wallpapers-hardy`: Edgy, Feisty, Gutsy, and Hardy
  * `xubuntu-wallpapers-dapper`: Dapper

## Hardware Support
* Bluetooth headphones are now better supported under PipeWire ([2017818](https://bugs.launchpad.net/ubuntu/+source/xubuntu-meta/+bug/2017818)) with the addition of `libspa-0.2-bluetooth`
* Recent touch input devices, including the second-generation Apple Magic Trackpad, are now supported with the removal of `xserver-xorg-input-synaptics`

## Updates

_Significant package and version updates. For full package changelogs, see the Changelogs section below._
...

## Changelogs
