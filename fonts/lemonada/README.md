# Worklog: Lemonada
Last Updated: Tuesday November 5th

## Basic Info
Arabic/Latin Typeface

## Project Links
| Relevant Links             | URLs                                                                                     |
| ------------------         | :--------------------------------------------------------------------------------------- |
| Working Git Repository     | [https://github.com/eliheuer/Lemonada](https://github.com/eliheuer/Lemonada)             |
| Upstream Git Repository    | [https://github.com/Gue3bara/Lemonada](https://github.com/Gue3bara/Lemonada)             |
| Google Fonts Page          | [https://fonts.google.com/specimen/Lemonada](https://fonts.google.com/specimen/Lemonada) |
| Google/fonts Pull Request  | [https://github.com/google/fonts/pull/1952](https://github.com/google/fonts/pull/1952)   |

## Work Status
- [x] Merged to [google/fonts](https://github.com/google/fonts)
- [ ] Changes requested on [github](https://github.com/google/fonts/pull/1952)

## Worklog
### Tuesday November 5th, 2019
```

Pull request was merged!

Built with ttfautohint setting: --stem-width-mode=nnn

To rebuild, clone this repo:

https://github.com/eliheuer/Lemonada/tree/gf-update
@ commit: ef5b2a24ed9966433fb10d652e638909ed86120b

And, then run the following line from the root directory:

sources/scripts/build.sh && sources/scripts/pull-request.sh

```
### Monday November 4th, 2019
```
REVIEWING LATEST PROOFS:

[ ] --stem-width-mode=nnn
    - Notes:looks ok but not great, matve better than deafault.
    - What are the other options?
    - There is too much weight change in Waterfall Desktop_Windows_10_firefox_62.0_.gif
    - Waterfall Desktop_OS_X_High_Sierra_safari_11.1_.gif looks okish.

```
### Wednesday October 30th, 2019
```
small proofing edits
decomposed braceright
```
### Thursday September 12th, 2019
```
[?] making sure OS/2 weightClass is fixed

[x] Name table script works
  - Checked in 

[x] Fixed gaf issue
  - commited update to gf-update branch

### Tuesday September 10th, 2019

[ ] Foo
  - Bar
```
### Monday September 9th, 2019
```
[ ] Adding name IDs 16 and 17 since it is a non-RIBBI font
  - RIBBI = (regular, italic, bold, bold italic)
  - https://glyphsapp.com/tutorials/naming
  - https://github.com/google/fonts/pull/1952
  - https://typedrawers.com/discussion/689/how-to-add-name-table-entries-with-fonttools

  - Work Notes
    - F
```
### Thursday September 5th, 2019
```
- [x] Tring to fix FB issues:
  - [ ] FAIL: Is the Grid-fitting and Scan-conversion Procedure ('gasp') table set to optimize rendering?
  - [ ] FAIL: Font is missing the 'gasp' table. Try exporting the font with autohinting enabled.
  - [x] FAIL: Does the font have a DSIG table?
    - [x] Fixing in build script
  - [ ] FAIL OS/2 sTypoDescender and hhea descent must be equal. [code: descender]
    - [ ] Changed winDescent from 651 to

- [x] OS/2 weightClass should be 300 (note from Marc)
  - [x] Added weightClass=300 custom parameter to the default Light master
  - !!! Note, info here: https://github.com/googlefonts/fontmake/issues/540
```
### Wednesday September 4th, 2019
```
- [ ] Tring to fix FB issues:
  - FAIL: Is the Grid-fitting and Scan-conversion Procedure ('gasp') table set to optimize rendering?
  - FAIL: Font is missing the 'gasp' table. Try exporting the font with autohinting enabled.
  - [ ] FAIL: Does the font have a DSIG table?
    - [ ] Fixing in source
```
### Tuesday September 3rd, 2019
```
- [x] Updated Lemonada PR
    - https://github.com/google/fonts/pull/1952

- [x] Add build scripts
    - sources/scripts/build.sh: builds variable font
    - sources/scripts/pull-request.sh: updates the google fonts repo

- [x] Add missing required codepoints: uni00AD & uni2215
    - uni00AD: SOFT HYPHEN
    - uni2215: DIVISION SLASH
```
### Thursday August 29th, 2019
```
- [ ] Update PR with reguested fixes
- [x] Make a new branch called `gf-update
```
### Wednesday August 28th, 2019
```
- [x] Move worklog
```
## Notes
```
gftools fix-fsselection Font-Regular.ttf --autofix
```
