# EmulationStation

This is your Root EmulationStation folder.

## .emulationstation

This folder contains your config files, Roms, gamelists and media. It also contains the ES Themes.

## Launch .Bat Files

By default when Windows ES opens it takes up the whole screen, and the only way to get it to go away is by pressing the Windows button (or closing the application).

Place these .bat files in the root of your EmulationStation folder and use one of them to open the program instead.

The 5 main included .bat files are:
- Launch ES 4x3 (1024x768).bat
- Launch ES Small Size (1024x576).bat
- Launch ES Mid Size (1280x720).bat
- Launch ES Full Size (1920x1080).bat
- Launch ES Fullscreen.bat (This one will launch ES in full screen instead of windowed no matter the size screen you are using. Does not work for 4K screens).

There are also 4 Debug .bat files that open a second "debug" window that gives you lots of useful information. It also lets you do the following things:
- Ctrl-R in a GamelistView will reload that view (including the theme)
- Ctrl-R in a SystemView will reload everything.
- Ctrl-G will toggle the lines of ComponentGrid.
- Ctrl-T will show bounding boxes around text elements, to debug text flow and filling and such.

I mostly use the Mid Size to create my themes and use the others for testing in the final stages.

These .bat files may not work if your file path contains a space or parentheses eg: `C:\Program FIles (x86)\Emulationstation`. Make the ES path clean eg: `C:\Emulationstation` and you shouldn't have a problem.

> The code for these .bat files originally came from [@herb_fargus's](https://retropie.org.uk/forum/user/herb_fargus) Portable ES build.
