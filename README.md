# ORC

ORC turns an SSL UF1 into a remote control for RME TotalMix FX. The fader, the pots and the keys
move TotalMix directly, and the two screens show what TotalMix is doing: channel names and colours,
levels, the EQ, reverb and echo. ORC runs in the menu bar and needs no DAW.

ORC is free.

**[Download the latest version](https://github.com/acklin83/ORC/releases/latest)** ·
**[Manual](https://acklin83.github.io/ORC/)**

## What you need

- A Mac with macOS 13 or later, Apple silicon or Intel.
- An SSL UF1, connected by USB.
- An RME interface with TotalMix FX 2.1 or later.

SSL 360° has to be closed while ORC uses the UF1.

## Setting up

1. In TotalMix, under Settings, OSC: set Compatibility Mode to Global OSC and switch Enable OSC
   Control on under Options.
2. Pick a free remote, tick *In Use*, and set IP `127.0.0.1`, *Port incoming* `7005`,
   *Port outgoing* `7006`. For the meters on the UF1, switch *Send Peak Level* on too.
3. Open the disk image and drag ORC to Applications.
4. Quit SSL 360°, connect the UF1, start ORC.

The [manual](https://acklin83.github.io/ORC/#setup) has the details.

## With Rea-Sixty

If you use [Rea-Sixty](https://github.com/acklin83/Rea-Sixty) in REAPER on the same Mac, REAPER
takes the UF1 over from ORC when it starts and hands it back when it quits. This needs Rea-Sixty
0.6.1 or later. See [ORC and Rea-Sixty](https://acklin83.github.io/ORC/#reasixty) in the manual.

## Problems

Open an [issue](https://github.com/acklin83/ORC/issues). The menu bar item says who holds the UF1
and whether TotalMix answers; please add those two lines.

## Licence

ORC's source code is published under the MIT License as part of
[Rea-Sixty](https://github.com/acklin83/Rea-Sixty). ORC ships libusb under the LGPL 2.1; its
source code is attached to the release. Details in
[THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).

SSL, UF1 and SSL 360 are trademarks of Solid State Logic. ORC is not affiliated with Solid State
Logic or RME.
