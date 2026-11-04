# ORC

ORC turns an SSL UF1, an SSL UF8 or both into a remote control for RME TotalMix FX. On the UF1, the
fader, the pots and the keys move TotalMix directly, and the two screens show what TotalMix is doing:
channel names and colours, levels, the EQ, reverb and echo. The UF8, next to the UF1 or on its own,
shows eight TotalMix channels on its faders, or drives Philips Hue lamps and DynaMount mic stands, and OBS
scenes can sit on the soft keys. ORC runs in the menu bar on a Mac, in the notification area on
Windows, and needs no DAW.

With MoreMe, musicians mix their own headphones on a phone or tablet: each picks Phones 1 to 4
and sets level, pan, mute and solo of every source in that mix, in a web page. Nothing is installed
on the phones.
Studio Control gives each musician a link of their own: their output, their faders, what they may
change.

ORC is free.

**[Download the latest version](https://github.com/acklin83/ORC/releases/latest)** ·
**[Manual](https://acklin83.github.io/ORC/)**

## What you need

- A Mac with macOS 13 or later, Apple silicon or Intel, or a 64-bit PC with Windows 11 or Windows 10
  version 1903 or later.
- An SSL UF1, an SSL UF8, or both, connected by USB.
- An RME interface with TotalMix FX 2.1 or later.

SSL 360° has to be closed while ORC uses the surfaces.

## Setting up

1. In TotalMix, under Settings, OSC: set Compatibility Mode to Global OSC and switch Enable OSC
   Control on under Options.
2. Pick a free remote, tick *In Use*, and set IP `127.0.0.1`, *Port incoming* `7005`,
   *Port outgoing* `7006`. For the meters on the UF1, switch *Send Peak Level* on too.
3. On a Mac, open the disk image and drag ORC to Applications. On Windows, run the installer:
   [Windows](https://acklin83.github.io/ORC/#windows) in the manual has the USB driver, the firewall and
   what Windows may say about an installer that is not code-signed.
4. Quit SSL 360°, connect the UF1 or the UF8, start ORC.

The UF1 shows the channels TotalMix shows: hide a channel there and ORC skips it.

MoreMe needs a second remote in TotalMix (ports 7003 and 7004) and is switched on in ORC's
settings, page MoreMe. See [MoreMe](https://acklin83.github.io/ORC/#moreme) in the manual.

The [manual](https://acklin83.github.io/ORC/#setup) has the details.

## With Rea-Sixty

If you use [Rea-Sixty](https://github.com/acklin83/Rea-Sixty) in REAPER on the same computer, REAPER
takes the UF1 and the UF8 over from ORC when it starts and hands them back when it quits, and Hue,
DynaMount and OBS settings stay in step between the two. This needs Rea-Sixty 0.8.0 or later
(0.6.1 or later for the UF1 alone), and 0.9.0 for ORC's assigned submix keys and the submix bank
while REAPER has the UF8. On Windows it needs Rea-Sixty 0.9.1 or later. See [ORC and Rea-Sixty](https://acklin83.github.io/ORC/#reasixty) in the manual.

## Problems

Open an [issue](https://github.com/acklin83/ORC/issues). ORC's menu says who holds the UF1
and whether TotalMix answers; please add those two lines.

## Licence

ORC's source code is published under the MIT License as part of
[Rea-Sixty](https://github.com/acklin83/Rea-Sixty). ORC ships libusb under the LGPL 2.1; its
source code is attached to the release. Details in
[THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).

SSL, UF1 and SSL 360 are trademarks of Solid State Logic. ORC is not affiliated with Solid State
Logic or RME.
