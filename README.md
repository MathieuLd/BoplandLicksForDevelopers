# BoplandLicksForDevelopers [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

## Description
This repository contains a collection of musicXML jazz licks (melodic segments) that were retrieved from the [BopLand](https://www.bopland.org/) website.

The licks are classified in 4 category :
- bass-clef-licks
- guitar-licks
- treble-clef-licks
- walking-bass-lines

Repository organization :

- `lick/image` contains the `.png` partition version of the licks
- `lick/jsonTag` contains for each category a json files providing tagging information for every licks
- `lick/musicXML` contains the actual `.xml` files providing the musical data (only treble-clef-licks and walking-bass-line are presents because bass-clef-licks, guitar-licks and treble-clef-licks are redundant, they contains the same licks but noted with the corresponding clef/notations)

## Why / How
When I tried to contact BopLand devs to ask if they could share their lick library in a more developer friendly format, I got no answer. So I decided to retrieve them myself and share them in case someone else had the same idea.

On the website, the licks are stored as .png partitions. To retrieve the musical data from these images the Optical Music Recognition software [Audiveris](https://github.com/Audiveris/audiveris) was used.

Python was used to automate all this process, I made a bunch of scripts that took care of the web scraping, the Audiveris mxl export and the mxl to xml conversion.

![alt text](images/bopland2xml.png "MusicXML retriving diagram")


This collection is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].


[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
