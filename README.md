# Choplifter Reverse-Engineer

This is a full reverse engineer of the Apple II game Choplifter, written by Dan Gorlin in 1982. It was done clean-room style beginning only with the binary. I had no additional information about this game other than the disk image.

The source code here is fully documented and will build and run to a version of Choplifter that is binary-identical to the original, except for Dan Gorlin's custom floppy loader. In order to modernize this a bit, I wrote a new loader for it based on ProDOS, and this version boots Choplifter from ProDOS instead. Otherwise, it is identical.

For a full writeup about this reverse-engineer and how it was done (along with lots more information about this source code), see my blog post here:

[https://blondihacks.com/reversing-choplifter/](https://blondihacks.com/reversing-choplifter/)

If you just want to look at the source code, it's all in choplifter.s (with zeropage locations in their own file for easier reference). There's also a makefile that will build this. If you're on a Mac, there's also an AppleScript that make can call which will launch Virtual II and boot the game. The ALL CAPS files are the graphics data which is ripped from the original disk image. The disk image in this archive (CHOPLIFTER.po) is bootable on any Apple II and contains the game compiled from my source. The disk image is assembled from parts using [cadius]([https://github.com/mach-kernel/cadius). Thanks to [Brutal Deluxe](http://brutaldeluxe.fr/products/crossdevtools/cadius/index.html) for this essential Apple II development tool.

This reverse engineer was completed by me, Quinn Dunki, on May 12, 2024, but this is of course still Dan's game and it is a brilliant piece of work. Reverse engineering it only *increased* my admiration of it. I doubt anyone would say that about most of what I've written in my career. 😁

Thanks Dan, for writing one of the best games on the platform, and I hope you don't mind that I did this to it.

