Linksys WAG200G tools
=====================

This repository contains some binaries and tools that will run on the Linksys WAG200G router.
It also contains a SquashFS image of the root filesystem with the "TCP-32764 backdoor" removed.

Please read http://blog.quarkslab.com/tcp-backdoor-32764-or-how-we-could-patch-the-internet-or-part-of-it.html for more information.

Files 

* src/squashfs2.2-lzma.patch: Patch for the SquashFS 2.2 release for LZMA support

* src/squashfs2.2-lzma/ : full sources for the SquashFS 2.2 LZMA tool

  Just do "make" in the squashfs-tools directory to compile it! Tested with GCC
  4.8 on 64-bit debian systems.

* binaries/nc: netcat compiled for MIPSLE:
  
   md5: a80d11b62d3e824eef416bd9a33413f7

   sha256: c6e24d54c142b25d6be82802d3e0bacd7a5412819a36df9854933adf619855f0

* binaries/mksquashfs2.2-lzma: SquashFS 2.2 with LZMA support

  md5: 04837bd1f906e207bcb53ccd54f84a2a

  sha256: 2a11d84de3f05eb5e4c34bd4247c137e06dc358b8c0d3560e0b2bc30e647c4d4

* binaries/unsquashfs4.0: SquashFS 4.0 with LZMA (Eloi's hack)

  md5: d17b78d7563c0b8c95288d53ec9728d9

  sha256: d1215fef8c168efb010aaeccec24989451a850c9c0ccf63dedd5eba1b8284cf5

* rootfs/original.img: original dump of the root filesystem

  md5: adcee0087cc3616a12af74cd522cfc7f

  sha256: a1f4ceea7b6e619044acb3c32e6b7792fcab44042b6bfe0e69448a0b1c8c265f

* rootfs/nobackdoor.img: original root filesystem without the TCP-32764 backdoor

  md5: f4eadf0a9173d5786c242afc80fdf20e

  sha256: 355cc96460ad1beeba8890bd89ce14daeba19dab35c0df9efa3ec441d9f194f0
