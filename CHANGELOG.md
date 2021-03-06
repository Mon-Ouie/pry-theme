Pry Theme changelog
===================

### v0.0.10 (July 07, 2012)

* Themes can use any color from 256-color palette as background color. Before
  this release you could use only 8 colors;
* Changed command flag `--list --remote` to `--remote-list`. Now, to get a list
  of themes from Pry Theme Collection, you type `pry-theme -r` or
  `pry-theme --remote-list` instead of `pry-theme -lr`;
* Limited theme descriptions to 80 characters;
* Added "content" subparameter for "string" parameter (`.prytheme` syntax).
* Changed the appearance of output from `pry-theme --all-colors` command, so it
  displays data in 3 columns instead of 1;
* Changed some colors of Railscasts and Tomorrow themes;
* Fixed bug when a user installs fresh gem and gets an improper warning, because
  `Pry.config.theme` is not defined. Added a proper notification message for
  such situations;
* Renamed default theme `charcoal-black` to `pry-cold` (they are not the same).

### v0.0.9 (July 05, 2012)

* **HOT**: Added `--install` flag. Now, you can easily install Pry themes from
  Pry Theme Collection via command line (`pry-theme -i nifty-theme`);
* Added pager for long output. Try `pry-theme -a 256` and you will immediately
  notice the difference;
* Added more informative output for `--list` flag;
* Added a bunch of new default themes: solarized, zenburn, twilight, tomorrow,
  saturday, railscasts, monokai, github and charcoal-black;
* Fixed wrong color name in 256-color palette (`pale_conflower_blue` →
  `pale_cornflower_blue`);
* Fixed bug with respect to unwanted fall back to the `pry-classic` theme,
  when a user tries to switch to nonexistent theme;
* Added a feature to `pry-theme` command: when a user invokes `pry-theme`
  command without arguments, it returns name of the current theme.

### v0.0.8 (July 02, 2012)

* **IMPORTANT**: Changed directory where to store themes! Themes now live in
  `$HOME/.pry/themes` directory on Mac OS and GNU/Linux, both. Do not forget
  to delete or move your themes form the old path (On Mac OS it is
  `$HOME/Library/Application Support/pry-theme` and on GNU/Linux it is
  `$HOME/.pry/themes`).
* On some operating systems Pry Theme was failing to detect correct config path.
  Fixed.
* Fixed wrong behaviour, when uninstalling an unrelated gem. Pry Theme asked to
  uninstall themes every time you wanted to uninstall _any_ gem.
* Fixed a typo in `pry-classic` theme, which was preventing to set `delimiter`
  parameter to a string.
* Fixed wrong convertation of theme files.
* Implemented `--list` (`-l`) option, which displays a list of all installed
  themes.

### v0.0.7 (June 30, 2012)

* **HOTFIX**: v0.0.6 is broken (because of my inattentiveness).

### v0.0.6 (June 30, 2012)

* Fixed bug when a `prytheme` attribute has no color value, but with attributes
  (for example, `symbol : (b)`);
* Fixed bug when a `prytheme` has no color value at all (for example,
  `symbol : `);
* Add basic checking for a valid color in `prytheme`.

### v0.0.5 (June 29, 2012)

* No pre!
* Added Ruby 1.8.7, JRuby and Ruby Enterprise Edition support;
* Fixed 8-color themes bug. We could not even use them in the previous version;
* Added `--test` command, which allows to "test" your theme visually;
* Added uninstaller, which basically just asks a user if he or she wants to
  remove a directory with Pry themes (personally, I hate when software leave
  their crap);
* Slightly improved `help` of `pry-theme` command;
* Made theme attributes optional. Now, if you are not sure about some parameter
  in a Pry Theme, you can leave it empty.

Last but not least:

  * Check out new Wiki! (https://github.com/kyrylo/pry-theme/wiki).

### v0.0.4.pre (June 28, 2012)

* Added `--all-colors` and `--color` options for `pry-theme` command;
* Improved used experience when working with `pry-theme`.

### v0.0.3.pre (June 26, 2012)

* Added support for Mac OS and Windows (I believe so, at least).

### v0.0.2.pre (June 26, 2012)

* Fixed bug with wrong detection of the root directory of the project.

### v0.0.1.pre (June 26, 2012)

* Initial release.
