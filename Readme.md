
# mad(1)

  `mad(1)` is a markdown driven manual page viewer,
  this makes manuals easier to _write_, _reuse_, and
  _read_.

  ![markdown man page](http://f.cl.ly/items/2G271F3c0D3p2i2V3l3k/Screen%20Shot%202012-04-14%20at%2012.44.58%20PM.png)

## Usage

    Usage: mad <file>

    Options:

      -u, --update    update remote mad-pages
      -V, --version   output cpm version
      -h, --help      output this help information

## Installation

  Install `mad(1)` and its associated mad page.

    $ make install

  Uninstall both `mad(1)` and the associated mad page.

    $ make uninstall

## About

  I _love_ man pages, however they are annoying to write by hand,
  and often converted from markdown anyway. `mad(1)` is effectively
  the same idea, but write your manuals in markdown like you would anyway,
  re-use them in your github readmes, wikis, or use markdown to HTML conversion
  tools.

  `mad(1)` pipes to `less(1)` so you get the same paging / searching
  goodness that you expect from `man(1)`.

## Page repository

  [mad-pages](https://github.com/visionmedia/mad-pages) is a collection of
  useful mad pages such as language operator precedence tables, http status
  codes, mime type tables etc.

## Page lookup

  Use the __MAD_PATH__ environment variable to control
  where `mad(1)` will look for a manual page.
  The ".md" extension may be omitted.

  For example:
  
    MAD_PATH="/usr/share/mad:share/mad"

  The following paths will always be searched:
  
     - .
     - /usr/local/share/mad
     - /usr/share/mad

## Screenshots

  Jade manual:
  
  ![jade manual markdown](http://f.cl.ly/items/3g1v2W213S2N390B201q/Screen%20Shot%202012-04-14%20at%201.54.35%20PM.png)