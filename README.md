# OpenDrive-Genesis
A open hardware flashcart for the Sega Genesis/32X

This project was born as way to use 3.3V parts safely for repro carts but, with the use o Flash memory, the read/write potencial of the ROM made me develop it to another direction: A Flashcart

This is quite a barebones Flashcart, nothing compared to Krizz's Everdrive ease of use. It is intended for DIY entusiasts, as learning platform and maybe as a starting point for me and other people projects. This is Open Hardware, do whatever it pleases you with it, I'm happy to help as needed.

As of now, these are its features:

- Suports Genesis and 32X software
- ROM Support for up to 4MB
- Save support for all ROM sizes (Selection for <2MB/>2MB by jumper)
- 32KB of FeRAM for saving
- No need for battery for saving
- Safe 3.3V to 5V level-shifting

What it doesnt do compared to commercially available carts:
- Multiple ROMs at the same time;
- ROM menu;
- SD support;
- Needs a programmer (The OpenDrive Programmer)
- Does not support Sega CD games and special chips (and probably never will);

This project is possible thanks to TmEE (NESdev Forums, SRAM wiring schematics), Rene Richard (db-electronics on GitHUB, KiCAD libs for the Genesis cart connector), lidnariq (NESdev Forums, Safe level-shifting), Ziggy587 (Racketboy, ideas, sugestions, support and encouragement), The Racketboy and NESdev forums.
