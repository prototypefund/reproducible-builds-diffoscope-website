---
layout: default
title: "diffoscope: in-depth comparison of files, archives, and directories"
---

# diffoscope

<div class="lead">In-depth comparison of files, archives, and directories.</div>

*diffoscope* will try to get to the bottom of what makes files or directories different. It will recursively unpack archives of many kinds and transform various binary formats into more human readable form to compare them. It can compare two tarballs, ISO images, or PDF just as easily.

----

<img src="/static/images/progressbar.gif?{{ site.time | date: '%s%N' }}">

## Examples

[![Example of diffoscope HTML output](/examples/https-everywhere-5.0.6_vs_5.0.7.thumbnail.png?{{ site.time | date: '%s%N' }})](/examples/https-everywhere-5.0.6_vs_5.0.7.html)

[Firefox extensions compared (HTML output)](/examples/https-everywhere-5.0.6_vs_5.0.7.html)

[![Example of diffoscope text output](/examples/igerman98_20131206-5.thumbnail.png?{{ site.time | date: '%s%N' }})](/examples/igerman98_20131206-5.txt)

[Debian packages compared (text output)](/examples/igerman98_20131206-5.txt)

&hellip; and more [examples on tests.reproducible-builds.org](https://tests.reproducible-builds.org/debian/unstable/amd64/index_FTBR.html).

## Features

* Command-line interface

* Text and HTML ouput

* Supported file formats: Android APK files, Android boot images, Berkeley DB database files, ColorSync colour profiles (.icc), Coreboot CBFS filesystem images, Dalvik .dex files, Debian .buildinfo files, Debian .changes files, Debian source packages (.dsc), Device Tree Compiler blob files, ELF binaries, FreeDesktop Fontconfig cache files, FreePascal files (.ppu), GHC Haskell .hi files, GIF image files, GNU R Rscript files (.rds), GNU R database files (.rdb), Gettext message catalogues, Git repositories, Gnumeric spreadsheets, Gzipped files, ISO 9660 CD images, JPEG images, JSON files, Java .class files, JavaScript files, LLVM IR bitcode files, MacOS binaries, Microsoft Windows icon files, Microsoft Word .docx files, Mono 'Portable Executable' files, Ogg Vorbis audio files, OpenOffice .odt files, OpenSSH public keys, OpenWRT package archives (.ipk), PDF documents, PGP signed/encrypted messages, PNG images, PostScript documents, RPM archives, Rust object files (.deflate), SQLite databases, SquashFS filesystems, TrueType font files, XML binary schemas (.xsb), XML files, XZ compressed files, ar(1) archives, bzip2 archives, character/block devices, cpio archives, directories, ext2/ext3/ext4/btrfs filesystems, statically-linked binaries, symlinks, tape archives (.tar), tcpdump capture files (.pcap) and text files.

* Fallback on hexdump comparison

* Fuzzy-matching to handle renamings

* &hellip; and many more!

## Get diffoscope

* **<a href="https://try.diffoscope.org/">Try it online!</a>**
* Via <a href="https://pypi.python.org/">`pip`</a>:<br /> `pip install diffoscope`<br /> *Note:* You might still want to install Python modules from <a href="https://github.com/trendmicro/tlsh">tlsh</a> and <a href="http://rpm.org/">rpm</a> and other external tools to get more meaningful results. Use `diffoscope --list-tools` to get the full list.

* On <a href="https://www.debian.org/">Debian</a> and derivatives:<br />
`apt install diffoscope`

* On <a href="https://fedoraproject.org">Fedora</a> based systems:<br/>
`dnf install diffoscope`

* On <a href="https://archlinux.org">Arch Linux</a>:<br/>
`pacman -S diffoscope`

* On <a href="http://brew.sh/">Homebrew</a>:<br/>`brew install diffoscope`

* <a href="/archive">Source tarballs</a>

* Through Git:<br />
`git clone https://salsa.debian.org/reproducible-builds/diffoscope.git`

## Contribute

*diffoscope* is developed within the <a href="https://reproducible-builds.org/">“Reproducible builds” effort</a>.

* <a href="https://salsa.debian.org/reproducible-builds/diffoscope">Git repository</a>

* <a href="https://salsa.debian.org/reproducible-builds/diffoscope/issues">Issues and feature requests</a>
  * <a href="https://salsa.debian.org/reproducible-builds/diffoscope/issues/new">File a new issue!</a> (<a href="https://reproducible-builds.org/contribute/salsa/">registration instructions</a>)

* <a href="https://lists.reproducible-builds.org/listinfo/diffoscope">Users and developers mailing-list</a>

* `#reproducible-builds` and/or `#debian-reproducible` on <a href="https://oftc.net/">OFTC</a>

Extending *diffoscope* to support new formats is quite straightforward in most cases. It also has a comprehensive test suite. Patches welcome!

## Similar software

* <a href="https://github.com/lvc/pkgdiff">pkgdiff</a>

* `pkg-diff.sh` from <a href="https://github.com/openSUSE/build-compare">Open Build Service build-compare</a>

## License

*diffoscope* is free software licensed under the <a href="https://www.gnu.org/licenses/gpl.html">GNU General Public License version 3</a> or later.

## Contributors

Lunar, Reiner Herrmann, Chris Lamb, Helmut Grohne, Holger Levsen,
Mattia Rizzolo, Daniel Kahn Gillmor, Paul Gevers, Peter De Wachter,
Yasushi SHOJI, Clemens Lang, Ed Maste, Joachim Breitner, Mike McQuaid.
Baptiste Daroussin, Levente Polyak, Ximin Luo, Maria Glukhova, Daniel Shahaf,
Juliana Oliveira Rodrigues.

