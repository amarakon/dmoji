Dmoji – Dmenu Emoji
================

## Contents

-   [Usage](#usage)
-   [Dependencies](#dependencies)
-   [Installation](#installation)
    -   [Universal](#universal)
    -   [Gentoo](#gentoo)
-   [Uninstallation](#uninstallation)
    -   [Universal](#universal-1)
    -   [Gentoo](#gentoo-1)

Dmoji is a simple program to select an emoji and copy it to the system
clipboard

## Usage

``` sh
`# user` dmoji -i # select an emoji
`# user` dmoji -n # select a unicode number
```

The `-i` option is used by default. Please run
`` `# user` dmoji --help `` for more information.

## Dependencies

1.  Dmenu
2.  Xclip

## Installation

### Universal

``` sh
`# user` git clone https://github.com/amarakon/dmoji
`# user` cd dmoji
`# root` make install
```

### Gentoo

``` sh
`# root` eselect repository add amarlay git https://github.com/amarakon/amarlay
`# root` emerge --sync amarlay
`# root` emerge x11-misc/dmoji
```

## Uninstallation

### Universal

``` sh
`# user` cd dmoji
`# root` make uninstall
```

### Gentoo

``` sh
`# root` emerge -c x11-misc/dmoji
# Remove my overlay (optional)
`# root` eselect-repository remove -f amarlay
`# root` emerge --sync
```
