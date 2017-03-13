#Universal XML Scraper

The [Universal XML Scraper](https://github.com/Universal-Rom-Tools/Universal-XML-Scraper) is a great tool that can scrape all metadata, images and videos for a large number of Systems. It pulls all the info from screenscraper.fr.

You can use Scrape Profiles to grab specific data/media and create custom gamelist.xml files. You can also use MIX Profiles to create custom images that combine multiple media into a single image.

Eg: This image combines a Screenshot, Logo and 3D Box-art.

![image from UXS](https://raw.githubusercontent.com/Universal-Rom-Tools/Universal-XML-Scraper/master/Images/Presentation/MIX/Super%20Mario%20All-Stars%20(Europe)-image.png)

Provided here are multiple Scrape and MIX Profiles that fulfil various purposes.

##Scrape Profiles

Scrape Profiles are placed in the "ProfilsFiles" folder of UXS. They are used to download the selected media and metadata, and use it to create a gamelist.xml. The Images in the "Ressources" folder are what you see in UXS when you have a specific Scrape Profile selected.

###Mattrixk [all media].xml
This Scrape Profile will download the following Media and place them into the gamelist.xml in the following tags:
```
Screenshot  - <screenshot>Aladdin-screenshot.jpg</screenshot>
3D Box-art  - <boxart3d>Aladdin-boxart3d.png</boxart3d>
2D Box-art  - <boxart2d>Aladdin-boxart2d.jpg</boxart2d>
Fan Art     - <fanart>Aladdin-fanart.jpg</fanart>
Logo        - <logo>Aladdin-logo.png</logo>
Cartridge   - <cartridge>Aladdin-cartridge.png</cartridge>
Video       - <video>Aladdin-video.mp4</video>
```

Notice the type of image has been appended to each item? This is because the Media all download to the same folder, so it keeps it nice and neat (I don't like having a different folder for each type of image).

Also note that some files are .jpg and some are .png (and the video is .mp4). This is because while some images (such as Logo and 3D Box-art) need to be .png for transparency, others are better left as .jpg.

This Scrape Profile does *not* create any MIX Images. It also isn't that useful for creating gamelists, as most of the `<Tags>` used don't actually exist. It is mainly useful for getting all the different Media available for each Rom to do with as you please.

###Mattrixk [video].xml
This Scrape Profile will download the following Media and place them into the gamelist.xml in the following tags:
```
MIX Image   - <marquee>Aladdin-mix-video.png</marquee>
Screenshot  - <image>Aladdin-screenshot.jpg</image>
Video       - <video>Aladdin-video.mp4</video>
```

This Scrape Profile is to be used in conjunction with the "Mattrixk (video).zip" MIX Profile.

###Mattrixk [no-video].xml
This Scrape Profile will download the following Media and place it into the gamelist.xml in the following tag:
```
MIX Image   - <image>Aladdin-mix-no-video.jpg</image>
```

This Scrape Profile is to be used in conjunction with the "Mattrixk (no-video).zip" MIX Profile.

> The maximum size of any image using these Scrape Profiles is 1024x1024. If images are smaller than this, they will *not* grow to meet it, but will remain at their original size (eg: a Screenshot will remain at 640x480).

##MIX Profiles

MIX Profiles are the fun ones that create a single image from multiple images. They are placed in the "Mix" folder of UXS. There are 2 MIX Profiles provided here; one for use with "Mattrixk [video].xml", and one for use with "Mattrixk [no-video].xml".

###Mattrixk (video).zip
Use this MIX Profile if you plan on using the "Mattrixk [video].xml" Scrape Profile. This MIX Profile will download the Logo, 3D Box-art and Cartridge, and combine them into a single 512x512 image that looks like this:

![image](https://github.com/mattrixk/es-toolkit/blob/master/emulationstation/downloaded_images/snes/Super%20Street%20Fighter%20II%20(USA)-mix-video.png)

The Screenshot/Video will sit in the middle of this MIX Image.

###Mattrixk (no-video).zip
Use this MIX Profile if you plan on using the "Mattrixk [no-video].xml" Scrape Profile. This MIX Profile will download the Logo, Screenshot, 3D Box-art and Cartridge, and combine them into a single 512x512 image that looks like this:

![image](#)

> A good thing to keep in mind is that the Videos from screenscraper.fr are 640x480 and between 3MB-15MB, so I wouldn't suggest putting too many on your RPi, as I don't know how well it would handle it. I'm in the process of trying to find a good way to reduce them using [Handbrake](https://handbrake.fr/), and if I find a way, I'll add the config to this Repo.
