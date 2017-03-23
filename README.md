# EmulationStation Toolkit
*A Toolkit full of little Extra bits for EmulationStation on Windows.*

---

**This is a work in progress. Some parts of the Toolkit are still missing. I'm steadily working on it and it should hopefully be complete soon**

---

I've put this Toolkit together to help people that want to start making themes for EmulationStation and RetroPie (and possibly RecalBox too. I haven't tried it, so I don't know how much help any of this will be for them).

It's basically a starting point that contains (fake\*) Roms with pre-scraped metadata, images and videos so you can just jump right in and start creating.

**Items in this Toolkit include:**
- Bat files to launch ES in different Windowed sizes.
- 100 (fake\*) Roms over 5 Systems: Gameboy, Gameboy Advance, N64, NES and SNES (20 Roms each).
- Scraped metadata, artwork and ~~videos~~\** for each every Rom.
- Custom Scrape and MIX Profiles for the [Universal XML Scraper](https://github.com/Universal-Rom-Tools/Universal-XML-Scraper/).
- A custom Theme that supports Video Previews and the Carousel Mod.
  
All images, logos and videos have been scraped with the Universal XML Scraper

>\* **There are no real Roms in this Repo.** They are just .txt files that have been renamed to match real games from their respective Systems. If you want real Roms you will have to find them yourself, I can't help you with that.

>\** The Videos took up too much room, so I moved them to their own Repo. You can get them from [ES Toolkit - Videos](https://github.com/mattrixk/es-toolkit-videos).

## Portable ES Builds

So far I've found 3 different versions of EmulationStation that you can download and use on Windows without too much hassle:
- [Portable ES](https://github.com/HerbFargus/Portable-Game-Station/releases/tag/1.3.6) by [@herb_fargus](https://retropie.org.uk/forum/user/herb_fargus).
  This version is the one that got me started. It's an older version that doesn't have any of the nifty new features like Video Previews, but it does have all the required Retroarch files to actually let you play the games. As such, it's a much larger download than the others in this list (about 150MB if I remember correctly).
- [Video Preview](https://github.com/fieldofcows/EmulationStation/releases/tag/v0.1-beta.7) by [@fieldofcows](https://retropie.org.uk/forum/user/fieldofcows).
  This version lets you use the new Video Previews functionality. The download is about 50MB.
- [Carousel Mod](https://dl.dropboxusercontent.com/u/859248/RetroPieES/SystemCarousel_mod_beta_22feb2017.7z) by [@Zigurana](https://retropie.org.uk/forum/user/Zigurana).
  This version lets you style the carousel in the System View, which is AWESOME. It also has Video Preview functionality, but before it will work you need the "plugins" folder from the "Video Preview" mod listed above. This download is only about 5MB, so if you don't care about playing games, or having working Videos, then this is the one for you.
  
I would recommend maybe just downloading all of them, then adding the "plugins" folder from "Video Preview" to "Carousel Mod", and adding the Retroarch files from "Portable ES" to "Carousel Mod" to make a super install that does it all!

>Note: I haven't tried adding the retroarch files, so I don't know if there is more to it than that. I can guarantee however that putting the "plugins" folder into "Carousel Mod" will get the Video Previews to work.
