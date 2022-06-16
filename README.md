# Dmoji – Dmenu Emoji

Dmoji is a simple program to select an emoji and copy it to the system clipboard
Its usage is simple:

* `$ dmoji -i` – select an emoji
* `$ dmoji -n` – select a unicode number

The `-i` option is used by default.

## Dependencies
1. dmenu
1. xclip

## (Un)Installation
### Universal
#### Installation
##### Latest Git Master (Bleeding Edge)
1. Git clone the repository.
* `$ git clone https://github.com/Amarakon55/dmoji`
2. Change working directory to *dmoji*.
* `$ cd dmoji`
3. Install Dmoji using the Makefile
* `# make install`
#### Uninstallation
##### Latest Git Master (Bleeding Edge)
1. Change working directory to *dmoji*.
* `$ cd dmoji`
2. Uninstall Dmoji using the Makefile
* `# make uninstall`

### Gentoo
#### Installation
##### Latest Git Master (Bleeding Edge)
1. Add my personal [Gentoo overlay](https://github.com/Amarakon55/amarlay) using [eselect-repository](https://packages.gentoo.org/packages/app-eselect/eselect-repository)
* `# eselect repository add amarlay git https://github.com/Amarakon55/amarlay`
2. Sync my personal [Gentoo overlay](https://github.com/Amarakon55/amarlay) using `emerge`
* `# emerge --sync amarlay`
3. Emerge the Dmoji package
* `# emerge x11-misc/dmoji` or `# emerge dmoji`
#### Uninstallation
##### Latest Git Master (Bleeding Edge)
1. Unmerge the Dmoji package
* `# emerge -c x11-misc/dmoji` or `# emerge -c dmoji`
2. (Optional) Remove my overlay
* `# eselect-repository remove -f amarlay`
3. (Optional) Sync using `emerge`
* `# emerge --sync`
