## What are "alternative" MEGA65 cores?

From day one, the MEGA65 was designed to be the spiritual successor of the legendary Commodore 65.
But the MEGA65 is much more than "just" that. It is also a MEGA versatile FPGA-based machine, a **chameleon**, that can turn itself into
any other machine you can imagine. All you need to peform this feat is a "alternative" MEGA65 core.

Please note: An alternative MEGA65 core is **not** an emulation of a certain hardware. Instead, it is a rebuild of the actual hardware itself.
Admittedly in most cases not a 100% exact rebuild. But still in general much better than any software emulator.

<img src="https://raw.githubusercontent.com/sy2002/m65cores/gh-pages/doc/retro.png">

Oliver Graf made a [great YouTube explainer video](https://youtu.be/9Ib7z64z9N4) about recreating retro systems using FPGAs,
about the awesome MiSTer project and about the difference between MiSTer and the equally awesome MEGA65. Watch the video
before reading on here, as it will provide you with valuable context.

## What alternative MEGA65 cores are available?

|                             |Alternative Core             |Status            |HDMI |VGA |3.5mm Audio  |MEGA65 File Host Link |Project page
|:----------------------------|:----------------------------|:-----------------|:----|:---|:------------|:---------------------|:--------------
| <img src="https://raw.githubusercontent.com/MJoergen/C64MEGA65/master/doc/c64.jpg" width="200">                       | **Commodore 64**                | In Development   | yes | yes | yes | n/a | [Click here](https://github.com/MJoergen/C64MEGA65)
| <img src="https://raw.githubusercontent.com/sy2002/gbc4mega65/master/doc/gb-and-gbc.jpg" width="200">                 | **Game Boy and Game Boy Color** | Fully functional | yes | yes | yes | [Download here](https://files.mega65.org?id=03b68172-d6ff-49f0-971e-15bea2c6ad9a) | [Click here](https://github.com/sy2002/gbc4mega65/)
| <img src="https://raw.githubusercontent.com/sy2002/zxuno4mega65/master/doc/wiki/assets/ZXSpectrum48k.jpg" width="200">| **ZX Spectrum**                 | Fully functional | no  | yes | yes | [Download here](https://files.mega65.org?id=bdaeb7e0-9fc8-4185-99de-104d01229f27) | [Click here](https://github.com/sy2002/zxuno4mega65)

## How do I install an alternative MEGA65 core?

1. Copy the `.cor` file on an SD card and insert it into the MEGA65
2. Make sure your MEGA65 is turned off
3. Press and hold the <kbd>NO SCROLL</kbd> key in the top row at position 5
4. Turn on your MEGA65
5. Press <kbd>CTRL</kbd> + <kbd>1</kbd> (or another number) to select the slot where you'd like to install the alternate core.
   You do not need to worry: You can change the slot at a later stage and you cannot overwrite your factory MEGA65 core and brick your machine.
6. Select the `.cor` file on your SD card

[Download the MEGA65 starter guide](https://files.mega65.org/news/MEGA65-Starter-Guide.pdf) and read the section `Bitstream Utility` to learn more.

## How do I run an alternative MEGA65 core?

1. Turn off your MEGA65
2. Press and hold the <kbd>NO SCROLL</kbd> key in the top row at position 5
3. Choose the core that you would like to run

## Can I add a core to this list?

Please message me on Discord (`sy2002#5425`), write me an email to `code` at `sy2002` dot `de`,
create an [Issue](https://github.com/sy2002/m65cores/issues) or create a [Pull Request](https://github.com/sy2002/m65cores/pulls),
if you think this list is incomplete and/or want me to add your project (work-in-progress projects are welcome!).

## How can I create an alternative MEGA65 core?

The [MiSTer Project](https://github.com/MiSTer-devel/Main_MiSTer/wiki) is the world's largest retro computing FPGA project. To see how many cores
they have, just go to their [Wiki pages](https://github.com/MiSTer-devel/Main_MiSTer/wiki), scroll down and look under the headline **FPGA Cores**
on the right side. It is stunning! :-)

So more than enough work for all you MEGA65 enthusiasts out there: Porting MiSTer cores is the logical first step and a great start when it comes
to building a decent library of alternative cores for the MEGA65. The Commodore 64 core and the Game Boy core from our list above are two great
examples of this.

For making your life easier, the [MiSTer2MEGA65 Framework](https://github.com/sy2002/MiSTer2MEGA65) will be there to simplify porting MiSTer cores to the MEGA65.
Beware! Currently, [MiSTer2MEGA65](https://github.com/sy2002/MiSTer2MEGA65) is heavily work in progress. Contributors welcome!
