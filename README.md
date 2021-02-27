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

# Other projects of the same family
- OpenDrive Programmer: https://github.com/soniccd123/OpenDrive-Programmer
- OpenDrive Programmer firmware: https://github.com/soniccd123/OpenDrive-Programmer-firmware
- OpenDrive Editor: https://github.com/soniccd123/OpenDrive-Editor

# Building the cartridge
I recommend that the release folder is used, the Bill of Materials is contained in the CSV file. The develop folder also works and its the actually tested cart by me, it only has aditional footprints for a being tested bank switching circuit.

The FM1808 is also not strictly necessary if you don't plan to save your games. The 74HC74 and the 74HC139 are still necessary in this case for the correct CE signaling.

You must short the JP1 jumper acordinly to the type of games you're going to use:
- For save support on <2MB games, short pins 1 and 2 (<2MB on the cart);
- For save support on >2MB games, short pins 3 and 2 (>2MB on the cart);
- If the save support is not necessary and the FM1808 is not soldered, short the 3 and 2 pins (>2MB on the cart).

With this the cart should be ready for writing and playing!

# Documentation
- Technical Manual, in constant work, sugestions welcome: https://docs.google.com/document/d/e/2PACX-1vTHuY665FCTQgpWVqtx0Hk3dTyNgIxMEns0RzGF2l86pw4OjIR6taxs3owxL13b5aOQaE71-1f7qCdJ/pub
- MX29L3211 Datasheet: http://www.wolfgangrobel.de/electronics/datasheets/eprom/MX29L3211.pdf
- FM1808 Datasheet: https://datasheet.octopart.com/FM1808-70-PG-Ramtron-datasheet-8328945.pdf
- 74HC74 Datasheet: https://assets.nexperia.com/documents/data-sheet/74HC_HCT74.pdf
- 74HC139 Datasheet https://assets.nexperia.cn/documents/data-sheet/74HC_HCT139.pdf
- 74LVC8T245 Datasheet: https://assets.nexperia.com/documents/data-sheet/74LVC_LVCH8T245.pdf

# Disclaimer
I'm not a professional hardware engineer, while this flashcart was designed to be the safest possible to your console, I'm not responsible for any damages done if used or built wrong. Also, revise the design always before building the PCB, I'm a amateur human and errors may have been commited. It you spot anything, hit me with a message and I will happily fix that. Also, any sugestions are welcome!
