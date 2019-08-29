# Worklog: Lemonada
Last Updated: Thu Aug 29th

## Table of Contents
* [Basic Info](#basic-info)
* [Project Links](#project-links)
* [Work Status](#work-status)
* [Worklog](#worklog)
* [FontBakery Status](#fontbakery-status)
* [Notes](#notes)

## Basic Info
Arabic/Latin Typeface

## Project Links
| Main Links     | URLs                                                                                     |
| -------------- | :--------------------------------------------------------------------------------------- |
| Origin repo    | [https://github.com/eliheuer/Lemonada](https://github.com/eliheuer/Lemonada)             |
| Upstream repo  | [https://github.com/Gue3bara/Lemonada](https://github.com/Gue3bara/Lemonada)             |
| Google Fonts   | [https://fonts.google.com/specimen/Lemonada](https://fonts.google.com/specimen/Lemonada) |
| Pull request   | [https://github.com/google/fonts/pull/1952](https://github.com/google/fonts/pull/1952)   |

## Work Status
- [ ] Merged
- [ ] PR needs to be updated to fix a few issues from Marc (in progress)

## Worklog

### Thursday August 29th, 2019
- [ ] Update PR with reguested fixes

### Wednesday August 28th, 2019
- [x] Move worklog

## Upstream Fontbakery Report

Fontbakery version: 0.7.11

<details>
<summary><b>[12] Lemonada-Roman-VF.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Checking file is named canonically.</summary>

* [com.google.fonts/check/canonical_filename](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/canonical_filename)
* 🔥 **FAIL** The file 'Lemonada-Roman-VF.ttf' must be renamed to 'Lemonada[wght].ttf' according to the Google Fonts naming policy for variable fonts. [code: bad-varfont-filename]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check glyph coverage.</summary>

* [com.google.fonts/check/glyph_coverage](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage)
* 🔥 **FAIL** Missing required codepoints: 0x00AD (SOFT HYPHEN) and 0x2215 (DIVISION SLASH) [code: missing-codepoints]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Is the Grid-fitting and Scan-conversion Procedure ('gasp') table set to optimize rendering?</summary>

* [com.google.fonts/check/gasp](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/gasp)
* 🔥 **FAIL** Font is missing the 'gasp' table. Try exporting the font with autohinting enabled. [code: lacks-gasp]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Font enables smart dropout control in "prep" table instructions?</summary>

* [com.google.fonts/check/smart_dropout](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/smart_dropout)
* 🔥 **FAIL** The 'prep' table does not contain TrueType instructions enabling smart dropout control. To fix, export the font with autohinting enabled, or run ttfautohint on the font, or run the `gftools fix-nonhinting` script. [code: lacks-smart-dropout]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check if the vertical metrics of a family are similar to the same family hosted on Google Fonts.</summary>

* [com.google.fonts/check/vertical_metrics_regressions](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vertical_metrics_regressions)
* 🔥 **FAIL** Lemonada Roman: OS/2 sTypoDescender is 653 when it should be -653 [code: bad-typo-descender]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking OS/2 Metrics match hhea Metrics.</summary>

* [com.google.fonts/check/os2_metrics_match_hhea](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/os2_metrics_match_hhea)
* 🔥 **FAIL** OS/2 sTypoDescender and hhea descent must be equal. [code: descender]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking with ftxvalidator.</summary>

* [com.google.fonts/check/ftxvalidator](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ftxvalidator)
* 🔥 **FAIL** ftxvalidator output follows:

b"Lemonada Roman\n\tLemonada-Roman\n\t48C24C98|4.004;1KTF;Lemonada-Roman\n\tkATSFontTestTrueTypeFontData\n\tFatal Minor Info \n\tcom.apple.TrueType.cmap.usability\n\t\t\xe2\x80\x98cmap\xe2\x80\x99 table usability\n\t\tThis test ensures the \xe2\x80\x98cmap\xe2\x80\x99 table has at least one usable subtable.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.TrueType.hmtx.usability\n\t\t\xe2\x80\x98hmtx\xe2\x80\x99 table usability\n\t\tThis test ensures the horizontal metrics table, \xe2\x80\x98hmtx\xe2\x80\x99, is valid.\n\t\tMinor Info \n\t\t\thmtx: Glyph 1 has a width of 693; it should be zero\n\t\t\t\tkATSFontTestSeverityMinorError\n\t\t\thmtx: Glyph 87 has a width of 1026, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 118 has a width of 1099, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 200 has a width of 1030, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 201 has a width of 1030, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 266 has a width of 1117, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 297 has a width of 1109, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 377 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 381 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 385 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 391 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 395 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 399 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 432 has a width of 1482, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 433 has a width of 1536, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 434 has a width of 1033, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 436 has a width of 1482, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 437 has a width of 1536, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 438 has a width of 1033, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 440 has a width of 1517, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 441 has a width of 1695, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 442 has a width of 1204, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 443 has a width of 1028, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 444 has a width of 1517, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 445 has a width of 1695, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 446 has a width of 1204, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 447 has a width of 1028, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 448 has a width of 1107, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 449 has a width of 1283, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 450 has a width of 1205, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 451 has a width of 1029, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 452 has a width of 1107, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 453 has a width of 1283, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 454 has a width of 1205, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 455 has a width of 1029, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 464 has a width of 1162, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 465 has a width of 1246, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 468 has a width of 1162, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 469 has a width of 1246, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 472 has a width of 1162, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 473 has a width of 1246, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 476 has a width of 1106, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 477 has a width of 1200, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 480 has a width of 1106, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 481 has a width of 1200, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 485 has a width of 1073, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 487 has a width of 1073, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 488 has a width of 1010, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 490 has a width of 1263, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 491 has a width of 1359, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 492 has a width of 1010, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 494 has a width of 1973, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 495 has a width of 2069, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 496 has a width of 1720, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 497 has a width of 1624, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 526 has a width of 1041, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 527 has a width of 1106, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 538 has a width of 1034, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 539 has a width of 1098, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 540 has a width of 1034, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 541 has a width of 1098, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 544 has a width of 1034, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 545 has a width of 1098, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 548 has a width of 1034, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 549 has a width of 1098, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 567 has a width of 1634, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 604 has a width of 1049, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 605 has a width of 1002, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 606 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 709 has a width of 1116, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 710 has a width of 1609, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 714 has a width of 1082, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 720 has a width of 1301, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 730 has a width of 1154, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\tcom.apple.TrueType.loca.usability\n\t\t\xe2\x80\x98loca\xe2\x80\x99 table usability\n\t\tThis test ensures the glyph data location table, \xe2\x80\x98loca\xe2\x80\x99, is valid.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.TrueType.name.usability\n\t\t\xe2\x80\x98name\xe2\x80\x99 table usability\n\t\tThis test ensures the \xe2\x80\x98name\xe2\x80\x99 table is valid.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.TrueType.post.usability\n\t\t\xe2\x80\x98post\xe2\x80\x99 table usability\n\t\tThis test ensures the \xe2\x80\x98post\xe2\x80\x99 table is valid.\n\t\tFatal \n\t\t\tpost: The name data overflow the table bounds.\n\t\t\t\tkATSFontTestSeverityFatalError\n\tcom.apple.TrueType.usability\n\t\t\xe2\x80\x98sfnt\xe2\x80\x99 required tables\n\t\tThis test ensures the \xe2\x80\x98sfnt\xe2\x80\x99 has all the required tables.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.TrueType.head.structure\n\t\t\xe2\x80\x98head\xe2\x80\x99 table structure\n\t\tThis test ensures the structure of the header table, \xe2\x80\x98head\xe2\x80\x99, accords with the specification.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.TrueType.hhea.structure\n\t\t\xe2\x80\x98hhea\xe2\x80\x99 table structure\n\t\tThis test ensures the structure of the horizontal header table, \xe2\x80\x98hhea\xe2\x80\x99, accords with the specification.\n\t\tMinor \n\t\t\thhea: descent (-653) is greater than 60 percent of the em (1000)\n\t\t\t\tkATSFontTestSeverityMinorError\n\tcom.apple.TrueType.maxp.structure\n\t\t\xe2\x80\x98maxp\xe2\x80\x99 table structure\n\t\tThis test ensures the structure of the maximum profile table, \xe2\x80\x98maxp\xe2\x80\x99, accords with the specification.\n\t\tMinor \n\t\t\tmaxp: The maxZones field is equal to 1; it should be equal to 2\n\t\t\t\tkATSFontTestSeverityMinorError\n\t\t\tmaxp: The table\\U2019s maximum component depth is 3; fonts with maximum component depth greater than 1 may not work properly on Mac OS X\n\t\t\t\tkATSFontTestSeverityMinorError\n\tcom.apple.TrueType.name.structure\n\t\t\xe2\x80\x98name\xe2\x80\x99 table structure\n\t\tThis test ensures the \xe2\x80\x98name\xe2\x80\x99 table is structurally sound.\n\t\tMinor \n\t\t\t'name': Two name entries overlap:  name entry 7 (bytes 504-518) and name entry 20 (bytes 504-518)\n\t\t\t\tkATSFontTestSeverityMinorError\n\tcom.apple.TrueType.glyf.usability\n\t\t\xe2\x80\x98glyf\xe2\x80\x99 table structure\n\t\tThis test ensures the \xe2\x80\x98glyf\xe2\x80\x99 table is structurally sound.\n\t\tMinor Info \n\t\t\tglyf: Glyph 1 should have no visual appearance but does\n\t\t\t\tkATSFontTestSeverityMinorError\n\t\t\tglyf: Glyph 583 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 584 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 585 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 586 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 587 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 593 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 594 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 595 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 596 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 597 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 675 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 676 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 823 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 824 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\tcom.apple.TrueType.glyf.instructions\n\t\t\xe2\x80\x98glyf\xe2\x80\x99 table instructions\n\t\tThis test ensures the instructions embedded in a \xe2\x80\x98glyf\xe2\x80\x99 table are sound.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.duplicates\n\t\tDuplicate fonts\n\t\tThis test verifies the presence of installed fonts with the same name.\n\t\tNA\n\t\t\t(No messages)\n"


</details>
<details>
<summary>🔥 <b>FAIL:</b> Glyph names are all valid?</summary>

* [com.google.fonts/check/valid_glyphnames](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/valid_glyphnames)
* 🔥 **FAIL** The following glyph names do not comply with naming conventions: alef-ar.short, alef-ar.fina.short, dotlessbeh-ar, dotlessbeh-ar.fina, dotlessbeh-ar.medi, dotlessbeh-ar.init, dotlessfeh-ar, dotlessfeh-ar.fina, dotlessfeh-ar.medi, dotlessfeh-ar.init and 34 more.

 A glyph name may be up to 31 characters in length, must be entirely comprised of characters from the following set: A-Z a-z 0-9 .(period) _(underscore). and must not start with a digit or period. There are a few exceptions such as the special character ".notdef". The glyph names "twocents", "a1", and "_" are all valid, while "2cents" and ".twocents" are not.

</details>
<details>
<summary>🔥 <b>FAIL:</b> Font contains unique glyph names?</summary>

* [com.google.fonts/check/unique_glyphnames](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unique_glyphnames)
* 🔥 **FAIL** The following glyph names occur twice: ['uni0394']

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check code page character ranges</summary>

* [com.google.fonts/check/code_pages](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/os2.html#com.google.fonts/check/code_pages)
* 🔥 **FAIL** No code pages defined in the OS/2 table ulCodePageRange1 and CodePageRange2 fields.

</details>
<details>
<summary>⚠ <b>WARN:</b> Stricter unitsPerEm criteria for Google Fonts. </summary>

* [com.google.fonts/check/unitsperem_strict](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/unitsperem_strict)
* ⚠ **WARN** Even though unitsPerEm (1000) in this font is reasonable. It is strongly advised to consider changing it to 2000, since it will likely improve the quality of Variable Fonts by avoiding excessive rounding of coordinates on interpolations. [code: legacy-value]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check for points out of bounds.</summary>

* [com.google.fonts/check/points_out_of_bounds](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/glyf.html#com.google.fonts/check/points_out_of_bounds)
* ⚠ **WARN** The following glyphs have coordinates which are out of bounds:
	* ('uni0337', 21.1, 30.5)
	* ('uni0337', 18.0, 30.5) and ('uni0337', 25.200000000000003, 30.5)

This happens a lot when points are not extremes, which is usually bad. However, fixing this alert by adding points on extremes may do more harm than good, especially with italics, calligraphic-script, handwriting, rounded and other fonts. So it is common to ignore this message. [code: points-out-of-bounds]

</details>
<br>
</details>

### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS |
|:-----:|:----:|:----:|:----:|:----:|:----:|
| 0 | 10 | 2 | 72 | 6 | 70 |
| 0% | 6% | 1% | 45% | 4% | 44% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**

## Origin GF-Mastering Fontbakery Report

Fontbakery version: 0.7.11

<details>
<summary><b>[12] Lemonada-Roman-VF.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Checking file is named canonically.</summary>

* [com.google.fonts/check/canonical_filename](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/canonical_filename)
* 🔥 **FAIL** The file 'Lemonada-Roman-VF.ttf' must be renamed to 'Lemonada[wght].ttf' according to the Google Fonts naming policy for variable fonts. [code: bad-varfont-filename]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check glyph coverage.</summary>

* [com.google.fonts/check/glyph_coverage](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage)
* 🔥 **FAIL** Missing required codepoints: 0x00AD (SOFT HYPHEN) and 0x2215 (DIVISION SLASH) [code: missing-codepoints]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Is the Grid-fitting and Scan-conversion Procedure ('gasp') table set to optimize rendering?</summary>

* [com.google.fonts/check/gasp](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/gasp)
* 🔥 **FAIL** Font is missing the 'gasp' table. Try exporting the font with autohinting enabled. [code: lacks-gasp]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Font enables smart dropout control in "prep" table instructions?</summary>

* [com.google.fonts/check/smart_dropout](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/smart_dropout)
* 🔥 **FAIL** The 'prep' table does not contain TrueType instructions enabling smart dropout control. To fix, export the font with autohinting enabled, or run ttfautohint on the font, or run the `gftools fix-nonhinting` script. [code: lacks-smart-dropout]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check if the vertical metrics of a family are similar to the same family hosted on Google Fonts.</summary>

* [com.google.fonts/check/vertical_metrics_regressions](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vertical_metrics_regressions)
* 🔥 **FAIL** Lemonada Roman: OS/2 sTypoDescender is 653 when it should be -653 [code: bad-typo-descender]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking OS/2 Metrics match hhea Metrics.</summary>

* [com.google.fonts/check/os2_metrics_match_hhea](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/os2_metrics_match_hhea)
* 🔥 **FAIL** OS/2 sTypoDescender and hhea descent must be equal. [code: descender]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking with ftxvalidator.</summary>

* [com.google.fonts/check/ftxvalidator](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ftxvalidator)
* 🔥 **FAIL** ftxvalidator output follows:

b"Lemonada Roman\n\tLemonada-Roman\n\t48C24C98|4.004;1KTF;Lemonada-Roman\n\tkATSFontTestTrueTypeFontData\n\tFatal Minor Info \n\tcom.apple.TrueType.cmap.usability\n\t\t\xe2\x80\x98cmap\xe2\x80\x99 table usability\n\t\tThis test ensures the \xe2\x80\x98cmap\xe2\x80\x99 table has at least one usable subtable.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.TrueType.hmtx.usability\n\t\t\xe2\x80\x98hmtx\xe2\x80\x99 table usability\n\t\tThis test ensures the horizontal metrics table, \xe2\x80\x98hmtx\xe2\x80\x99, is valid.\n\t\tMinor Info \n\t\t\thmtx: Glyph 1 has a width of 693; it should be zero\n\t\t\t\tkATSFontTestSeverityMinorError\n\t\t\thmtx: Glyph 87 has a width of 1026, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 118 has a width of 1099, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 200 has a width of 1030, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 201 has a width of 1030, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 266 has a width of 1117, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 297 has a width of 1109, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 377 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 381 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 385 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 391 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 395 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 399 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 432 has a width of 1482, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 433 has a width of 1536, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 434 has a width of 1033, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 436 has a width of 1482, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 437 has a width of 1536, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 438 has a width of 1033, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 440 has a width of 1517, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 441 has a width of 1695, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 442 has a width of 1204, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 443 has a width of 1028, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 444 has a width of 1517, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 445 has a width of 1695, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 446 has a width of 1204, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 447 has a width of 1028, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 448 has a width of 1107, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 449 has a width of 1283, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 450 has a width of 1205, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 451 has a width of 1029, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 452 has a width of 1107, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 453 has a width of 1283, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 454 has a width of 1205, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 455 has a width of 1029, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 464 has a width of 1162, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 465 has a width of 1246, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 468 has a width of 1162, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 469 has a width of 1246, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 472 has a width of 1162, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 473 has a width of 1246, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 476 has a width of 1106, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 477 has a width of 1200, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 480 has a width of 1106, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 481 has a width of 1200, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 485 has a width of 1073, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 487 has a width of 1073, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 488 has a width of 1010, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 490 has a width of 1263, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 491 has a width of 1359, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 492 has a width of 1010, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 494 has a width of 1973, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 495 has a width of 2069, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 496 has a width of 1720, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 497 has a width of 1624, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 526 has a width of 1041, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 527 has a width of 1106, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 538 has a width of 1034, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 539 has a width of 1098, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 540 has a width of 1034, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 541 has a width of 1098, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 544 has a width of 1034, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 545 has a width of 1098, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 548 has a width of 1034, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 549 has a width of 1098, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 567 has a width of 1634, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 604 has a width of 1049, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 605 has a width of 1002, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 606 has a width of 1080, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 709 has a width of 1116, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 710 has a width of 1609, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 714 has a width of 1082, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 720 has a width of 1301, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\thmtx: Glyph 730 has a width of 1154, which is greater than the font\\U2019s em (1000); this may be incorrect.\n\t\t\t\tkATSFontTestSeverityInformation\n\tcom.apple.TrueType.loca.usability\n\t\t\xe2\x80\x98loca\xe2\x80\x99 table usability\n\t\tThis test ensures the glyph data location table, \xe2\x80\x98loca\xe2\x80\x99, is valid.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.TrueType.name.usability\n\t\t\xe2\x80\x98name\xe2\x80\x99 table usability\n\t\tThis test ensures the \xe2\x80\x98name\xe2\x80\x99 table is valid.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.TrueType.post.usability\n\t\t\xe2\x80\x98post\xe2\x80\x99 table usability\n\t\tThis test ensures the \xe2\x80\x98post\xe2\x80\x99 table is valid.\n\t\tFatal \n\t\t\tpost: The name data overflow the table bounds.\n\t\t\t\tkATSFontTestSeverityFatalError\n\tcom.apple.TrueType.usability\n\t\t\xe2\x80\x98sfnt\xe2\x80\x99 required tables\n\t\tThis test ensures the \xe2\x80\x98sfnt\xe2\x80\x99 has all the required tables.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.TrueType.head.structure\n\t\t\xe2\x80\x98head\xe2\x80\x99 table structure\n\t\tThis test ensures the structure of the header table, \xe2\x80\x98head\xe2\x80\x99, accords with the specification.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.TrueType.hhea.structure\n\t\t\xe2\x80\x98hhea\xe2\x80\x99 table structure\n\t\tThis test ensures the structure of the horizontal header table, \xe2\x80\x98hhea\xe2\x80\x99, accords with the specification.\n\t\tMinor \n\t\t\thhea: descent (-653) is greater than 60 percent of the em (1000)\n\t\t\t\tkATSFontTestSeverityMinorError\n\tcom.apple.TrueType.maxp.structure\n\t\t\xe2\x80\x98maxp\xe2\x80\x99 table structure\n\t\tThis test ensures the structure of the maximum profile table, \xe2\x80\x98maxp\xe2\x80\x99, accords with the specification.\n\t\tMinor \n\t\t\tmaxp: The maxZones field is equal to 1; it should be equal to 2\n\t\t\t\tkATSFontTestSeverityMinorError\n\t\t\tmaxp: The table\\U2019s maximum component depth is 3; fonts with maximum component depth greater than 1 may not work properly on Mac OS X\n\t\t\t\tkATSFontTestSeverityMinorError\n\tcom.apple.TrueType.name.structure\n\t\t\xe2\x80\x98name\xe2\x80\x99 table structure\n\t\tThis test ensures the \xe2\x80\x98name\xe2\x80\x99 table is structurally sound.\n\t\tMinor \n\t\t\t'name': Two name entries overlap:  name entry 7 (bytes 504-518) and name entry 20 (bytes 504-518)\n\t\t\t\tkATSFontTestSeverityMinorError\n\tcom.apple.TrueType.glyf.usability\n\t\t\xe2\x80\x98glyf\xe2\x80\x99 table structure\n\t\tThis test ensures the \xe2\x80\x98glyf\xe2\x80\x99 table is structurally sound.\n\t\tMinor Info \n\t\t\tglyf: Glyph 1 should have no visual appearance but does\n\t\t\t\tkATSFontTestSeverityMinorError\n\t\t\tglyf: Glyph 583 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 584 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 585 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 586 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 587 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 593 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 594 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 595 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 596 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 597 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 675 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 676 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 823 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\t\t\tglyf: Glyph 824 has no visual appearance\n\t\t\t\tkATSFontTestSeverityInformation\n\tcom.apple.TrueType.glyf.instructions\n\t\t\xe2\x80\x98glyf\xe2\x80\x99 table instructions\n\t\tThis test ensures the instructions embedded in a \xe2\x80\x98glyf\xe2\x80\x99 table are sound.\n\t\tNA\n\t\t\t(No messages)\n\tcom.apple.duplicates\n\t\tDuplicate fonts\n\t\tThis test verifies the presence of installed fonts with the same name.\n\t\tNA\n\t\t\t(No messages)\n"


</details>
<details>
<summary>🔥 <b>FAIL:</b> Glyph names are all valid?</summary>

* [com.google.fonts/check/valid_glyphnames](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/valid_glyphnames)
* 🔥 **FAIL** The following glyph names do not comply with naming conventions: alef-ar.short, alef-ar.fina.short, dotlessbeh-ar, dotlessbeh-ar.fina, dotlessbeh-ar.medi, dotlessbeh-ar.init, dotlessfeh-ar, dotlessfeh-ar.fina, dotlessfeh-ar.medi, dotlessfeh-ar.init and 34 more.

 A glyph name may be up to 31 characters in length, must be entirely comprised of characters from the following set: A-Z a-z 0-9 .(period) _(underscore). and must not start with a digit or period. There are a few exceptions such as the special character ".notdef". The glyph names "twocents", "a1", and "_" are all valid, while "2cents" and ".twocents" are not.

</details>
<details>
<summary>🔥 <b>FAIL:</b> Font contains unique glyph names?</summary>

* [com.google.fonts/check/unique_glyphnames](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/unique_glyphnames)
* 🔥 **FAIL** The following glyph names occur twice: ['uni0394']

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check code page character ranges</summary>

* [com.google.fonts/check/code_pages](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/os2.html#com.google.fonts/check/code_pages)
* 🔥 **FAIL** No code pages defined in the OS/2 table ulCodePageRange1 and CodePageRange2 fields.

</details>
<details>
<summary>⚠ <b>WARN:</b> Stricter unitsPerEm criteria for Google Fonts. </summary>

* [com.google.fonts/check/unitsperem_strict](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/unitsperem_strict)
* ⚠ **WARN** Even though unitsPerEm (1000) in this font is reasonable. It is strongly advised to consider changing it to 2000, since it will likely improve the quality of Variable Fonts by avoiding excessive rounding of coordinates on interpolations. [code: legacy-value]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check for points out of bounds.</summary>

* [com.google.fonts/check/points_out_of_bounds](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/glyf.html#com.google.fonts/check/points_out_of_bounds)
* ⚠ **WARN** The following glyphs have coordinates which are out of bounds:
	* ('uni0337', 21.1, 30.5)
	* ('uni0337', 18.0, 30.5) and ('uni0337', 25.200000000000003, 30.5)

This happens a lot when points are not extremes, which is usually bad. However, fixing this alert by adding points on extremes may do more harm than good, especially with italics, calligraphic-script, handwriting, rounded and other fonts. So it is common to ignore this message. [code: points-out-of-bounds]

</details>
<br>
</details>

### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS |
|:-----:|:----:|:----:|:----:|:----:|:----:|
| 0 | 10 | 2 | 72 | 6 | 70 |
| 0% | 6% | 1% | 45% | 4% | 44% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**

## Notes
gftools fix-fsselection Font-Regular.ttf --autofix
