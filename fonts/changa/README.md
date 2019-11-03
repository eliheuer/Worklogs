# Worklog: Changa

Last Updated: Tue Aug 28th

## Table of Contents

* [Basic Info](#basic-info)
* [Project Links](#project-links)
* [Work Status](#work-status)
* [Worklog](#worklog)
* [FontBakery Status](#fontbakery-status)
* [Notes](#notes)

## Basic Info

Arabic/Latin Typeface

Needs a manual ttx fix after build:
Name table: Family name (id1) from ExtraLight to Changa ExtraLight

## Project Links

| Main Links     | URLs                                                                                   |
| -------------- | :------------------------------------------------------------------------------------- |
| Hard fork      | [https://github.com/eliheuer/changa-vf](https://github.com/eliheuer/changa-vf)         |
| Soft fork      | [https://github.com/eliheuer/Changa](https://github.com/eliheuer/Changa)               |
| Upstream repo  | [https://github.com/etunni/Changa](https://github.com/etunni/Changa)                   |
| Google Fonts   | [https://fonts.google.com/specimen/Changa](https://fonts.google.com/specimen/Changa)   |
| Pull request   | [https://github.com/google/fonts/pull/1949](https://github.com/google/fonts/pull/1949) |

## Work Status

- [ ] Done
- [ ] Marc requested a PR back to the upstream project
- [x] Working on a build script

## Worklog

### Week of October 1st
- [ ] Glyphs:
    - [x] The gaf bar is still broken.
    - [ ] Are the double combining vowel marks correct? I haven't checked them thoroughly.
        * Note: Not sure, come back to this later.

- [x] masters:
    - [x] change the master names from [regular, bold] to [extralight, extrabold].
        - this will fix the typographic name errors since it will generate the typo name records.
        - this needs to be set in this manner because of glyphslib.

- [x] instances:
    - [x] change the extralight weightclass to 200. i know fb produces a warn if it isn't 275 for static fonts, however, felipe is fixing this as we speak.

- [x] Build script:
    - [x] Update to our new VF filename schema

- [ ] Vertical metrics:
    - [ ] Difference on Windows may be occurring due to a glyph in the character set. You can use pyftsubset to try and track down which glyph may be triggering the metrics to be different.
        - We can't release this due to this issue. I'm more than happy to help you with this next week.

- [ ] FontBakery issues:
    - [x] FAIL: Missing required codepoints: 0x00AD (SOFT HYPHEN) and 0x2215 (DIVISION SLASH)
    - [ ] FAIL: Check name table: TYPOGRAPHIC_SUBFAMILY_NAME entries.
    - [ ] FAIL: Variable font weight coordinates must be multiples of 100.
    - [ ] FAIL: Check variable font instances have correct coordinate values
    - [ ] FAIL: Checking OS/2 Metrics match hhea Metrics.


### Thursday September 26th
- [x] PR has been updated
- [ ] FontBakery issues:
    - [ ] FAIL: Missing required codepoints: 0x00AD (SOFT HYPHEN) and 0x2215 (DIVISION SLASH)
    - [ ] FAIL: Check name table: TYPOGRAPHIC_SUBFAMILY_NAME entries.
    - [ ] FAIL: Variable font weight coordinates must be multiples of 100.
    - [ ] FAIL: Check variable font instances have correct coordinate values
    - [ ] FAIL: Checking OS/2 Metrics match hhea Metrics.
    - [x] FAIL: Glyph names are all valid?
          This issues isnt a big deal
          Save for last of dont fix.


### Wednesday September 25th
- [ ] Forked gabbers repo and updating build script and PR
    - [x] Adding build scripts: Done
    - [x] Now there is a fontmake error:
    - ValueError: Currently, we only support bracket layers that are present on all masters, i.e. what the Glyphs.app tutorial calls 'Changing All Masters'. There is a/are bracket layer(s) missing for glyph(s) ['Oslash', 'oslash', 'dollar'].
    - I fixed fixed the issue above in the source in my "gf-update" fork.


### Monday September 23rd
- [ ] Restaring work
    - [ ] There is a open pr from Gabber with work from Marc
    - [ ] The upstream repo seems unresponsive: maybe branch from gabers fork?
        - Notes on when each branch was last updated:
        - etunni/Changa/master ---- Jun 28, 2016
        - Gue3bara/Changa/master -- Jun 07, 2018
        - m4rc1e/Changa/all ------- All commits behind Gaber's fork


### Wednesday August 28th, 2019

- [ ] Looking into an upstream PR


## FontBakery Status

Nothing here.

## Notes

Nothing here.
