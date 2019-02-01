# PaperRenamer

Rename academic paper files to human friendly names with the paper titles.

![PaperRenamer Demo](demo.gif)

## Paper Renamer for MacOS

PaperRenamer for MacOS is a native MacOS application created from the modified Python script [pdftitle](https://github.com/huwan/pdftitle) using [Platypus](https://sveinbjorn.org/platypus). This is done by wrapping the script in a MacOS application bundle along with an executable binary that runs the script.

### Installation

**Available packages**

- Download the latest DMG file from releases page [here](https://github.com/huwan/PaperRenamer/releases).

- Double-click the DMG file to open it, and you’ll see a Finder window. Simply drag the application’s icon to your Applications folder and you’re done.

**Build and install manually**

We provide a profile which saves Platypus's configuration settings for building the application. All other necessary files (python script, pdftohtml tool, and icon files) can be found in the `Resources` directory.

- Install [Platypus](https://sveinbjorn.org/platypus).
- Double-click the profile `Paper Renamer.platypus` which have a .platypus filename suffix. Or launch Platypus and load the profile by selecting it from the menu (Profiles → Load Profile...).
- Click "Create App" to generate the application.
- Move the `Paper Renamer.app` to your Applications folder.

### Usage
Simply launch the `Paper Renamer.app`, drag and drop your pdf files to the square window. You can also open pdf files by selecting it from the menu.


## Paper Renamer for Linux

It's convenient to launch a Terminal to run the pdf rename python script in Linux. Here we introduce a better way to rename paper by adding drag and drop support to the script.

You can create .desktop file for the python script used here. With the .desktop file, you can drag and drop your paper pdfs to the desktop icon to rename papers. Please refer to  [this link](https://www.maketecheasier.com/create-desktop-file-linux) for more details on how to create a .desktop file in Linux.
Here is a sample .desktop file:

```
[Desktop Entry]
Name=PaperRenamer
Exec=/path/to/PaperRenamer/Resources/script %U
Type=Application
Icon=/path/to/PaperRenamer/Resources/AppIcon.png
Name[en_HK]=PDF Rename
```

## Credits

Thanks go to Uwe Dauernheim, the original author of the [pdftitle](https://github.com/djui/pdftitle) tool used for PDF article title extraction in Paper Renamer, Sveinbjorn Thordarson, author of [Platypus](https://sveinbjorn.org/platypus) which is a great developer tool that created this MacOS application from command line script, and Sindre Sorhus for [create-dmg](https://github.com/sindresorhus/create-dmg) tool that created a good-looking DMG for this app in seconds.

## Acknowledgements

* [poppler (pdftohtml)](https://poppler.freedesktop.org/), a PDF rendering library.
* [FreeType](https://www.freetype.org/), a freely available software library to render fonts.
* [Fontconfig](https://www.freedesktop.org/wiki/Software/fontconfig/), a library for configuring and customizing font access.
* [libjpeg](http://www.ijg.org/), a free library for JPEG image compression.
* [libpng](http://libpng.org/), the free reference library for reading and writing PNGs.
* [LibTIFF](http://www.libtiff.org/), a library for reading and writing TIFF.

## License

Code is licensed under the [BSD 2-Clause "Simplified" License](LICENSE). Icon made by [phatplus](https://www.flaticon.com/authors/phatplus) from [www.flaticon.com](https://www.flaticon.com) is licensed by [CC 3.0 BY](https://creativecommons.org/licenses/by/3.0/).
