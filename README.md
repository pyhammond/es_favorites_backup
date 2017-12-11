# es_favorites_backup

A group of scripts I wrote to allow you to backup your Favorites / Kids Games / Last Played XML data from [Emulation Station](https://github.com/Aloshi/EmulationStation) so you can run a [scraper](https://github.com/sselph/scraper) and update your `gamelist.xml` files without losing all of your favorites / kids games / last played / play counts, etc.

### Installation Instructions

Login to your Retropie box as the 'pi' user and simply run:

	(cd && git clone http://github.com/pyhammond/es_favorites_backup)

There are 4 scripts now in that `es_favorites_backup` directory.  They all begin with `fav_`.

The two scripts you really should care about are called `fav_backup` and `fav_restore`.  You may want to put all of these four files somewhere in your bin path like under `/usr/local/bin/`.

### fav_backup

Running this will simply parse through all of your `gamelist.xml` files and back up the contents into a saved data file.  You can then scrape any / all of your systems and restore the favorites aftward by calling `fav_restore`.

### fav_restore

This will simply restore all of your saved favorites / kids games / last played / play counts back into your `gamelist.xml` files system-wide after you have scraped and re-generated your `gamelist.xml` files used by [Emulation Station](https://github.com/Aloshi/EmulationStation).

### Credits

Thanks to [sselph](https://github.com/sselph) for creating such a great [scraper](https://github.com/sselph/scraper).