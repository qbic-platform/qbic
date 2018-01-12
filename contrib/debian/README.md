
Debian
====================
This directory contains files used to package qbicd/qbic-qt
for Debian-based Linux systems. If you compile qbicd/qbic-qt yourself, there are some useful files here.

## qbic: URI support ##


qbic-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install qbic-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your qbic-qt binary to `/usr/bin`
and the `../../share/pixmaps/qbic128.png` to `/usr/share/pixmaps`

qbic-qt.protocol (KDE)

