# Cal Sans 1.0

## Introduction
Cal Sans is a geometric sanserif tuned for display, that is, large point sizes. It is an Open Source typeface to adorn the headlines and interfaces of [Cal.com](https://cal.com/), a company founded by [Peer Richelsen](https://twitter.com/peer_rich) and [Bailey Pumfleet](https://twitter.com/BaileyPumfleet) and interface design by [Ciarán Hanrahan](https://twitter.com/CiaranHan).

The basis of Cal Sans is my initial answer to what my Futura would be. It fit well with Peer’s brief, for something serious and and geometric so that the letters of “cal.com” would have circular shapes throughout. It was decided early on that it be open source for all!

![Specimen Example](/documentation/images/blog-specimen.jpg)


## Design Philosophy and Unique Characteristics
As this design was created for display, and is currently a single static font, an unusual approach is taken for its texture and default typography. Letters are intentionally spaced to be extremely close for tight headlines “out of the box.” For smaller subheadings, positive letter spacing must be applied. There are currently no other Open Source geometric sanserifs geared as intentionally for “tight but not touching” typesetting—as it is more labor intensive to produce with accurate texture. But for typesetters, if they would letterspace another design as tight as Cal Sans, the results would not be as consistent.

![Open Source Fonts’ Default Spacing](/documentation/images/Default-Spacing.gif)

So, for end users, more flexibility is available when the tightest typesetting extreme edge case is gracefully addressed. One may create looser typesetting as needed.


## OpenType Features
While the default design is fairly ahistorical, there are historical design options. Using Stylistic Set 01 (ss01), Futura-specific alternates can be deployed. Including diacritic variants, there are 48 alternates for this set.

![A sample of ss01](/documentation/images/blog-specimen_ss01.jpg)

I give credit to [Rasmus Andersson](https://twitter.com/rsms) implementing in his design [Inter](https://github.com/rsms/inter) Character Variants to offer more control in website typography. Cal Sans also employs this feature. There are six Character Variants in Cal Sans, for **Cc (cv01)**, **j (cv02)**, **t (cv03)**, **u (cv04)**, **0 (cv05**, and **1 (cv06)**.

In celebration of Futura’s geometrically extreme ligatures, Cal Sans has an experimental approach to ligatures, Stylistic Set 02 (ss02) is identical to ss01, but also combines eligible letters as historical Futura ligatures. This is included as a stylistic set and not as discretionary ligatures because default characters really do not match these historical ligatures. (But they were included anyway!)

![A sample of ss02](/documentation/images/blog-specimen_ss02.jpg)

Probably the most novel OpenType feature of Cal Sans is its third Stylistic Set (ss03). The best way to exhibit the need of ss03 is to see how “tight but not touching” affects spacing with consecutive diagonals. Some designers would _never_ want their letters to overlap or touch in a headline, or very large title.

![Open Source Fonts’ Default Spacing](/documentation/images/ss03_kerning.gif)

Diagonals’ corners are kerned from eachother, and some might say this causes more problems than the “stock” kerning solves. Such letter combinations aren’t…incredibly common. But they are not rare, nor is spacing letters in a way that is sometimes consistent a goal of mine. But, I see merits in both paths. **So, ss03 overrides diagonal-to-diagonal kerning pairs with new ones that let diagonal corners “crash.”**


I don’t know of any other typefaces that has many kerning options, hopefully this feature is of use! Thanks to Tal Leming’s [OpenType Cook Book](https://opentypecookbook.com/rules/) for technical details.


## Usage Sample


```
h1 {font-size: 56px;}
h2 {font-size: 40px; letter-spacing: .01em;}
h3 {font-size: 36px; letter-spacing: .015em;}
h4 {font-size: 28px; letter-spacing: .02em;}
h5 {font-size: 20px; letter-spacing: .03em;}
h6 {font-size: 16px; letter-spacing: .04em;}
.quote {font-size: 24px; letter-spacing: .02em;}
.smaller_cal_sans {font-size: 18px; letter-spacing: 0.045em;}
```

## License

This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is copied below, and is also available with a FAQ at
http://scripts.sil.org/OFL

## Special Thanks
Thank you to Peer for commisioning this project, and for [Maxim Leyzerovich](https://twitter.com/round) for recommending me. I also wanted to shout out Bold Monday’s Futura Today, a design that I love. I wanted to also thank Wei Huang for his Open Source “Perfect Glyphs Example File” that is Work Sans dot glyphs. Incredibly helpful, and exhibits genius.

The following people were invaluable to this project, in no specific order, with an undisclosed amount of personal (or impersonal) influence:

* Mirko Velimirovic & Stephen “Thunder” Nixon
* Luke Shuman
* Paul Renner
* Roger Black, David Berlow, Tobias Frere-Jones, Matthew Carter, Jonathan Hoefler, Kris Sowersby
* Hannes Famira, Cara Di Edwardo, Andy Clymer, David Jonathan Ross, Troy Leinster, Thomas Jockin
* Jamaal Nelson, Florante Generoso, jen hung, Laura Van Wyk
* As Cal Sans is the fruit of my labor, I  am the fruit of Scott & Lori Davis


## Repository Layout

This font repository structure is inspired by [Unified Font Repository](https://github.com/googlefonts/Unified-Font-Repository), modified for the Google Fonts workflow.

## Installation Instructions
- [GNU+Linux](https://wiki.archlinux.org/index.php/fonts#Manual_installation)
- [MacOS](https://support.apple.com/en-us/HT201749)
- [Windows](https://support.microsoft.com/en-us/help/314960/how-to-install-or-remove-a-font-in-windows)
