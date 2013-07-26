typecatcher
===========

Grabs all the fonts from a Typekit and installs them.

#### Prerequisites

You have a Typekit kit created and you've added the domain "localhost" to it.

### Running the downloader
In order to download a TypeKit kit, run the following after cloning the repo:
```
ruby ~/path/to/repo/run.rb XXXXXXX
```
Where XXXXXXX is the 7 character Typekit code.

All fonts will be downloaded into the repo's `fonts` folder, as well as being installed in your system's font directory.

#### Notes on hidden font files
The files in the `/Library/Fonts` have the following hidden flag applied to them:
```
`chflags hidden /Library/Fonts/#{filename}.otf`
`chflags hidden /Library/Fonts/#{filename}.ttf`
```
So if you are looking for those files be aware that they are hidden.
