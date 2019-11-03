# Worklog: Lemonada
Last Updated: Sunday November 3rd

## Basic Info
Arabic/Latin Typeface

## Project Links
| Relevant Links     | URLs                                                                                     |
| ------------------ | :--------------------------------------------------------------------------------------- |
| Origin repo        | [https://github.com/eliheuer/Lemonada](https://github.com/eliheuer/Lemonada)             |
| Upstream repo      | [https://github.com/Gue3bara/Lemonada](https://github.com/Gue3bara/Lemonada)             |
| Google Fonts       | [https://fonts.google.com/specimen/Lemonada](https://fonts.google.com/specimen/Lemonada) |
| Pull request       | [https://github.com/google/fonts/pull/1952](https://github.com/google/fonts/pull/1952)   |

## Work Status
- [ ] Merged to [google/fonts](https://github.com/google/fonts)
- [x] Changes requested

## Worklog


### Wednesday October 30th, 2019
small proofing edits
decomposed braceright

### Thursday September 12th, 2019

[?] making sure OS/2 weightClass is fixed

[x] Name table script works
  - Checked in 

[x] Fixed gaf issue
  - commited update to gf-update branch

### Tuesday September 10th, 2019

[ ] Foo
  - Bar

### Monday September 9th, 2019

[ ] Adding name IDs 16 and 17 since it is a non-RIBBI font
  - RIBBI = (regular, italic, bold, bold italic)
  - https://glyphsapp.com/tutorials/naming
  - https://github.com/google/fonts/pull/1952
  - https://typedrawers.com/discussion/689/how-to-add-name-table-entries-with-fonttools

  - Work Notes
    - F

### Thursday September 5th, 2019

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

### Wednesday September 4th, 2019

- [ ] Tring to fix FB issues:
  - FAIL: Is the Grid-fitting and Scan-conversion Procedure ('gasp') table set to optimize rendering?
  - FAIL: Font is missing the 'gasp' table. Try exporting the font with autohinting enabled.
  - [ ] FAIL: Does the font have a DSIG table?
    - [ ] Fixing in source

### Tuesday September 3rd, 2019
- [x] Updated Lemonada PR
    - https://github.com/google/fonts/pull/1952

- [x] Add build scripts
    - sources/scripts/build.sh: builds variable font
    - sources/scripts/pull-request.sh: updates the google fonts repo

- [x] Add missing required codepoints: uni00AD & uni2215
    - uni00AD: SOFT HYPHEN
    - uni2215: DIVISION SLASH

### Thursday August 29th, 2019
- [ ] Update PR with reguested fixes
- [x] Make a new branch called `gf-update
### Wednesday August 28th, 2019
- [x] Move worklog

## Notes
gftools fix-fsselection Font-Regular.ttf --autofix
