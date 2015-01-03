VBA-SDL-H
=========

This is a fork of https://github.com/cosarara97/vba-sdl-h/
It was created in order to make vba-sdl-h compile on Arch Linux.
There is no support for creating png screenshots (only bmp) with this version, because
there were major version issues with libpng which denied me to compile vba-sdl-h.

Arch Linux AUR: https://aur.archlinux.org/packages/vba-sdl-h/

Original Notice
---------------

This is a fork of VBA-SDL-H, as a result of the author's repository having
been down for some time.

Vanilla VBA-SDL-H (see links at the bottom) wouldn't build on an updated arch
linux. The configure script couldn't be regenerated without bringing all that
autotools system to today's standards as well. I decided to just remove
the entire build system and write a short Makefile (which shouldn't be
too difficult to maintain).

Also, I applied these changes to fix a bug:

http://sourceforge.net/p/vba/patches/35/

Config
------

The configuration file is named VisualBoyAdvance.cfg, and will be installed
in /etc/ on "make install". You can copy it to ~/.config/vba-sdl-h/", and
it will take precedence over the former.

[1] http://labmaster.bios.net.nz/vba-sdl-h/

[2] https://www.dropbox.com/s/1bp33i7j2uxhlva/vba-sdl-h-src.tar.gz?dl=0
