# YASH

This is a Kosmo format version of René Schmitz's [YASH](https://www.schmitzbits.de/sah.html) sample and hold synth module.

The circuit is pretty much as Schmitz designed it. The only significant changes are the addition of an output jack for the clock signal, an attenuator for the input signal, and a switch to bypass the capacitor on the clock input. The latter turns the module from a sample and hold into a track and hold: applying a gate to the clock input causes the output to track the input voltage, and then when the gate turns off the last output voltage is held until the next gate.

## Current draw
11.3 mA +12 V, 4.0 mA -12 V


## Photos

![](Images/front.jpg)

![](Images/back.jpg)

## Documentation

* [Schematic](Docs/yash.pdf)
* PCB layout: [front](Docs/yash_layout_front.pdf), [back](Docs/yash_layout_back.pdf)
* [BOM](Docs/yash_bom.md)
* [Build notes](Docs/build.md)
* [Blog post](https://analogoutputblog.wordpress.com/2022/05/06/yet-another-sample-and-hold/)

## GitHub repository

* [https://github.com/holmesrichards/yash](https://github.com/holmesrichards/yash)

## Submodules

This repo uses submodules aoKicad and Kosmo_panel, which provide needed libaries for KiCad. To clone:

```
git clone git@github.com:holmesrichards/yash.git
git submodule init
git submodule update
```


Alternatively do

```
git clone --recurse-submodules git@github.com:holmesrichards/yash.git
```

Or if you download the repository as a zip file, you must also click on the "aoKicad" and "Kosmo\_panel" links on the GitHub page (they'll have "@ something" after them) and download them as separate zip files which you can unzip into this repo's aoKicad and Kosmo\_panel directories.

If desired, copy the files from aoKicad and Kosmo\_panel to wherever you prefer (your KiCad user library directory, for instance, if you have one). Then in KiCad, go into Edit Symbols and add symbol libraries 

```
aoKicad/ao_symbols
Kosmo_panel/Kosmo
```
and go into Edit Footprints and add footprint libraries 
```
aoKicad/ao_tht
Kosmo_panel/Kosmo_panel.
```
