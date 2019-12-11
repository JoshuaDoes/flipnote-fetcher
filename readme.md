## Flipnote Fetcher

Fetch Flipnotes from [Flipnote Hatena](http://ugomemo.hatena.ne.jp/thankyou) -- in 2019

## Wait, What?

After [Flipnote Hatena](http://ugomemo.hatena.ne.jp/thankyou) was closed down, Nintendo converted all user-created Flipnotes to make then accessible from [Flipnote Studio 3D's](https://www.nintendo.co.uk/Games/Nintendo-3DS-download-software/Flipnote-Studio-3D-763095.html) "DSi Library" feature. 

DSi Library was shut down when Nintendo closed the rest of Flipnote Studio 3D's online features, and along with it all of the content from Flipnote Hatena disappeared. 

Or so we thought! Luckily, the amazing folks over at [Internet Archive](http://web.archive.org/) made a backup!

This project uses a super-basic Python script to interact with Internet Archive's API and fetch all of the Flipnotes for a given user's Flipnote Studio ID. These Flipnotes can then be browsed and converted to video in [Flipnote Player](https://flipnote.rakujira.jp/).

## Usage

Requirements:
 * Python 3, tested on 3.7.4 but should work on other versions

To find how many Flipnotes are archived for a Flipnote Studio ID (e.g. 97849B20AA34FFBC)

```
python3 flipnote_fetcher.py 97849B20AA34FFBC 
```

To download all those Flipnotes, just pass a target directory as a second param:

```
python3 flipnote_fetcher.py 97849B20AA34FFBC ./downloads
```

## Caveats

Unfortunately, we're only able to fetch Flipnotes by Flipnote Studio ID. It’s not possible to search for a specific username or Hatena ID. If you’d like those features, you might want to wait for Austin Burk’s much more comprehensive [Flipnote Archive](https://twitter.com/FlipnoteArchive) project.

## Credits

* [James Daniel](https://jamesdaniel.dev) Python implementation
* [Shutterbug2000](https://github.com/shutterbug2000) Discovered the Internet Archive backup
* [Internet Archive](http://web.archive.org/)