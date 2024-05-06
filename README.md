Imagine you're on a train, in an area with poor cell reception. You look for available Wi-Fi networks, and there's one called "Come Get
This Wi-Fi". When you connect, you get a pop-up window that says, "Sorry, this network doesn't connect to the internet! Enjoy this essay!" And what follows is something you never would've read otherwise!

This zine will show you how to make your own wi-fi access point and web server using a Wemos D1 mini board. The Wemos D1 mini is small, cheap, and easy to program using the Arduino IDE.

# Details
The following zine was created for the workshop "Pocket Portal Power Play: Crafting Wi-Fi Access Points with a Twist", hosted for the first time at the [2024 Open Hardware Summit](https://2024.oshwa.org/).

The zine is a remix of the ["Spread ideas with a pocket wi-fi portal"](https://iffybooks.net/pocket-wifi-portal/) zine by [Iffy Books](https://iffybooks.net/about/), licensed under Anti-copyright, no rights reserved.

The zine has two versions: a digital version, and a quarter-page print-ready version. Both versions have the same dimensions (quarter of a US letter size sheet).

# Printing and Assembling the Zine

The print-version of the zine was generated using the incredible [Zine Arranger Tool by Nash High](https://html-classic.itch.zone/html/5825267-604447/ZineArranger/index.html) ([itch page](https://nashhigh.itch.io/zinearranger), [source code](https://github.com/romadox/zine-arranger)).

## Printing Setup

To prepare the zine, download the print-ready PDF version of the zine from the [repo](https://github.com/pocket-portal/zine). Send it for print with the following settings:
- US Letter sized paper
- 100% scale
- Double-sided (Flip on long edge)

Here's how those settings look like in Acrobat:

![Screenshot of print settings in Adobe Acrobat](https://i.imgur.com/4M9dgmY.png)

## Assembly
(Taken from the [Zine Arranger Printing Instructions](https://html-classic.itch.zone/html/5825267-604447/ZineArranger/folding.html?q2ps))

1. Once printed, keep sheets stacked in the order they printed.
2. Lay the pile with the front cover at the top right.
3. Cut the entire pile in half horizontally. A guillotine paper cutter will make this proccess much easier, especially if you're printing multiple zines.
4. Stack the top pile on top of the bottom. The front & back covers should be on top. Check the order of pages, making sure pages 14-15 and 42-43 follow each other.
5. Fold the whole stack in half left-to-right and staple/bind the spine.

![Zine assembly illustration by Nash High for the Zine Arranger](https://i.imgur.com/QUZWc3g.png)

# Editing the Zine

1. [Download the fonts](https://github.com/pocket-portal/zine/tree/main/fonts) used for the zine and install them on your computer: [Aileron](https://tipotype.com/underground/aileron/) and [Space Mono](https://www.colophon-foundry.org/custom-projects/space-mono).

2. Download the editable version `.docx` of the zine from the [repo](https://github.com/pocket-portal/zine).
   
3. Make your changes in the word processor of your choice. I used OnlyOffice to create this zine, but you can edit it with LibreOffice Writer, Word, etc.

4. Export the document as a PDF.

5. To prepare the zine for print, you could use a zine preparing tool like [Zine Arranger by Nash High](https://html-classic.itch.zone/html/5825267-604447/ZineArranger/index.html). Make sure that the final number of pages are a multiple of 8.
 Here are the settings I used to prepare the quarter zine for print in the Zine Arranger:
  ![Selected options in the Zine Arranger](https://i.imgur.com/o60w50O.png)

6. Once it's ready, refer to the [print and assembly instructions](#printing-and-assembling-the-zine).


# How is this different from the original?

The key difference between this zine and [Iffy Books's zine](https://iffybooks.net/pocket-wifi-portal/) is that the captive portal method uses a newer version of the Arduino IDE (2.x+) and the LittleFS filesystem instead of SPIFFS.

You can read more about the genesis of this remix here: [Issue with SPIFFS storage instructions (version 0.6) · Issue #2 · iffybooks/pocket-wifi-portal](https://github.com/iffybooks/pocket-wifi-portal/issues/2)

## Added:
+ Pocket Portal Power Play branding (fonts, graphics, colours)
+ "What you'll need" section
+ [Example code for captive portals](https://github.com/pocket-portal/code)
+ More examples of things you could do with the captive portal
+ QR codes to access zine source files and code examples
+ "Tips and Tricks" section
  + Optimizing media
  + Remove spaces in media
  + Remember to host all files on the board
+ "Further Ideas" section
  + Different ways of generating static sites
  + How to host the pages online instead
  + Ideas for advertising and prompting people to connect to the captive portal (Wi-Fi QR codes and NFC tags)

## Removed:
- OS-specific Arduino IDE installation instructions. *(I figured that the link to the download page would be enough, and will likely contain the latest instructions.)*
- LED blink example
- Captive portal approach 1: write HTML in the Arduino IDE *(I do reference it at the end, however)*

## Updated
- ~~References to SPIFFS~~ → Using [LittleFS Upload plugin by Earle F. Philhower, III](https://github.com/earlephilhower/arduino-littlefs-upload)
- ~~References to Arduino IDE version 1.8.x~~ → Arduino IDE 2.x
- Screenshots for the latest Arduino IDE version (2.3.2)
- License: this one is licensed under CC0 instead of Anti-copyright
- Minor updates to phrasing