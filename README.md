# ES-extras
Extra bits for EmulationStation on Windows

**This is a work in progress. Most parts are currently missing**

The idea behind this Repo is just to provide all the necessary bits for people who download one of the Windows ES builds like the [Video Preview](https://github.com/fieldofcows/EmulationStation/releases/tag/v0.1-beta.7) build by @fieldofcows or the [Carousel build](https://dl.dropboxusercontent.com/u/859248/RetroPieES/SystemCarousel_mod_beta_22feb2017.7z) by @Zigurana.

Extras include:
- Bat files to launch ES in different Windowed sizes
  - Full screen - 1920x1080
  - Mid screen - 1280x720
  - 4:3 - 1024x768
  
- Rom folders for multiple Systems, each with a number of fake roms. (Please note, these are just empty .txt files that have been renamed to match the expected file extensions. *THEY ARE NOT REAL ROMS*).

- Scraped images and videos for each of the included Systems and Roms.
  - Scraped images include Box-art, Fan-art, Logos, Screenshots and Cartridges (where available).
  - I have also included a basic MIX image from [UXS](https://github.com/Universal-Rom-Tools/Universal-XML-Scraper/) for each of the Roms.
  - The files are named like this:
    - Aladdin-boxart.png
    - Aladdin-fanart.jpg
    - Aladdin-screenshot.jpg
    - Aladdin-cartridge.png
    - Aladdin-logo.png
    - Aladdin-mix.png
    - Aladdin-video.mp4

- Gamelists for each of the included Systems and Roms.
  - All videos are within "video" tags.
  - All "image" tags are filled with the Screenshots.
  - All "marquee" tags are filled the Logos.

- A custom Theme that supports Video Preview.
  - This is a basic theme without much ornamentation, to be used as both a learning tool, and a base/starting point for your own theme.
  - This theme only supports the Systems that have Roms in this download.
  
- Custom Scrape and MIX Profiles for UXS
  - These are the profiles I used to scrape all the single images, videos and MIX images for each Rom.
  - You can add these profiles to your copy of UXS to scrape all your Roms to be same as those provided.
  - There are 2 Scrape Profiles and 2 MIX Profiles, one MIX Profile for each Scrape Profile.
    - Scrape-ES-extras-video.xml scrapes videos for each Rom (if available), and uses the MIX-ES-extras-video.zip to create a MIX image that uses Logo, 3D Box-art and Cartridge (if available).
    - Scrape-ES-extras-no-video.xml uses the MIX-ES-extras-no-video.zip to create a MIX image that uses Logo, Screenshot, 3D Box-art and Cartridge (if available).
  
All images, logos and videos have been scraped with the Universal XML Scraper
