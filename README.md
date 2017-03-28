# EmulationStation Toolkit
*A Toolkit for Making EmulationStation Themes*

---

**This is a work in progress.**

---

This kit includes:

- Launch (.bat) scripts for different screen sizes
- 100 (fake\*) Roms over 5 Systems: Gameboy, Gameboy Advance, N64, NES and SNES (20 Roms each).
- Scraped metadata, artwork and ~~videos~~\** for each every Rom.
- Custom Scrape and MIX Profiles for the [Universal XML Scraper](https://github.com/Universal-Rom-Tools/Universal-XML-Scraper/).
- A custom Theme that supports Video Previews and the Carousel Mod.

>Videos are kept in their own repository [HERE](https://github.com/mattrixk/es-toolkit-videos)

**NO ROMS or copyrighted content are included in this repository!**

## Installation

### Windows

See the [Releases](https://github.com/mattrixk/es-toolkit/releases) page to download the latest version.

You can extract it with 7zip and can be run on a USB stick.

The binaries in the release are compiled for windows only.

Note: because it is a portable build you will need to use the .bat scripts (not the executable) to launch ES.

### Linux 

The release only includes ES binaries for windows, but the configs from the toolkit can still be used on systems running linux such as RetroPie

```
git clone https://github.com/mattrixk/es-toolkit.git
```

For example with RetroPie you can copy:

es_systems.cfg to `/opt/retropie/configs/all/emulationstation/es_systems.cfg`

roms to `~/RetroPie/roms/`

themes to `/opt/retropie/configs/all/emulationstation/themes/`

You can see a guide on building EmulationStation on linux [Here](https://github.com/mattrixk/es-toolkit/wiki/Building-EmulationStation-on-Linux)

You can also run emulationstation with a different window size and resolution

`emulationstation --windowed --resolution 640 480`

### Acknowledgements

Special thanks to @fieldofcows for the video view and @Zigurana for the carousel mod. Both are now part of the RetroPie fork of EmulationStation and are included in the ES-Toolkit Releases

Thanks to Screech for UXS and Rookervik for his Theme Helper.

For those wanting a complete system with working emulators, @herbfargus configured a portable build with Retroarch and EmulationStation called [PortableGameStation](https://github.com/HerbFargus/Portable-Game-Station/releases/)

