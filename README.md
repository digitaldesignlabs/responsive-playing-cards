Responsive Playing Cards
========================

tldr; Responsive SVG playing cards. Most cards ~2K, picture cards are ~65k. With gzip, they’re about half that. When rendered <= 75px wide, they switch to a simpler layout for readability.

LGPL licensed.

Introduction
------------
This is a deck of SVG playing cards which was created for a client project in January 2015. The project is targeted specifically at Chromium, so the cards may not work on other platforms (pull requests welcomed).

The cards are based on the deck produced by [Chris Aguilar](https://code.google.com/p/vectorized-playing-cards/), hosted over at Google Code, with the exception of the Ace of Spades, which was taken from [Byron Knoll](https://code.google.com/p/vector-playing-cards/)’s public domain cards also at Google Code.

What do you get?
----------------
Each card has been hand-optimized to reduce the file size as far as possible, by re-using and transforming paths. This takes the size of a normal card down from ~6.5k to about ~2.5k (~1.7k minified, 800b minified + zipped).  Picture cards are obviously more complex, at ~90k (~65k minified, ~30k minified + zipped).

<div style="background:#efefef;padding:6px;max-width:790px">
  <img src="minified/diamonds/3d.svg" width="200" alt="Three of Diamonds, 200px wide" style="vertical-align:bottom;border-radius:4%;box-shadow:0 0 6px #ccc;margin-right:5px">
  <img src="minified/diamonds/3d.svg" width="160" alt="Three of Diamonds, 160px wide" style="vertical-align:bottom;border-radius:4%;box-shadow:0 0 6px #ccc;margin-right:5px">
  <img src="minified/diamonds/3d.svg" width="120" alt="Three of Diamonds, 120px wide" style="vertical-align:bottom;border-radius:4%;box-shadow:0 0 6px #ccc;margin-right:5px">
  <img src="minified/diamonds/3d.svg" width="80" alt="Three of Diamonds, 80px wide" style="vertical-align:bottom;border-radius:4%;box-shadow:0 0 6px #ccc;margin-right:5px">
  <img src="minified/diamonds/3d.svg" width="60" alt="Three of Diamonds, 60px wide" style="vertical-align:bottom;border-radius:4%;box-shadow:0 0 6px #ccc;margin-right:5px">
  <img src="minified/diamonds/3d.svg" width="40" alt="Three of Diamonds, 40px wide" style="vertical-align:bottom;border-radius:4%;box-shadow:0 0 6px #ccc;margin-right:5px">
  <img src="minified/diamonds/3d.svg" width="30" alt="Three of Diamonds, 30px wide" style="vertical-align:bottom;border-radius:4%;box-shadow:0 0 6px #ccc;margin-right:5px">
  <img src="minified/diamonds/3d.svg" width="20" alt="Three of Diamonds, 20px wide" style="vertical-align:bottom;border-radius:4%;box-shadow:0 0 6px #ccc">
</div>

The cards also have embedded media queries, which display a simpler layout if the card is scaled below 75px wide.

Platforms
---------
The cards are specified in SVG Tiny 1.2, and have been tested on Chrome 40, Firefox 35, Safari 8, Mobile Safari 8, Opera 11, Opera Classic for Android, Windows Phone 8.1, Internet Explorer 11 (Windows 7) and Internet Explorer 11 (Windows RT 8.1).

Bugs
----
The “mini” versions of the cards (< 75px) don’t render on Firefox for Android, or on Mobile Safari 6. Instead, the big cards are displayed.

Credits
-------

The original cards were created by Chris Aguilar. The Ace of Spades was by Byron Knoll.<br>
They were optimized by Mike Hall with help from Warren Lockhart.

License
-------

LGPL 3.0
