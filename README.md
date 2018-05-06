# Practical Typography fonts made practical

The fonts ship in a ZIP. By using scripts from this repository, you'll get
CSS files ready to be used on your website. You can include each CSS file
individually. It's one file per one font. Thus, if you need two font styles,
just concatenate the file.

# Preparing

1. Buy fonts from Matthew Butterick: https://practicaltypography.com/equity.html

2. Download them to ~/Downloads

3. Modify the `.settings` file. The release version of the fonts is here. Mine was `180117`. Your is probably different, so adjust it.

# Quickstart

Install tools:

	./mk.install

Then do:

	./mk.unpack
	./mk.rename
	./mk.fonts

# How it works

- `mk.unpack` unzips the files and moves them to a separate directory
- `mk.rename` makes all the directories and files not have any spaces in them (spaces make everything harder),  and be named in a consistent manner (without additional _ here and there)
- `mk.fonts` uses several command line tools to convert fonts to WOFF2, EOT and SVG parameters required by some browsers. 
