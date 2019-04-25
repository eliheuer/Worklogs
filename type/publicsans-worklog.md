
# Table of Contents

1.  [PUBLIC SANS WORKLOG](#org1788c6c)
    1.  [BASIC INFO](#org9a19068)
    2.  [FONTBAKERY STATUS](#org487908e)
        1.  [ROMAN](#org942d221)
        2.  [ITALIC](#org8ed5b39)
    3.  [S](#orgef99eb7)
        1.  [Close old PR](#org507cd35)
        2.  [Make GF-mastering branch](#org8dbf3f9)
        3.  [PR Public Sans](#org61e150d)
        4.  [PR Public Sans Italic](#orgbd4fbdd)
    4.  [BUILD HELPERS](#orged65776)
        1.  [FontBakery](#org932f3b0)
        2.  [Addfont](#orgb26ae80)
        3.  [Build Commands](#org0fd3b81)
        4.  [Build Info](#orga6a23d3)
    5.  [BUILD STEPS](#orgb4ba37a)
    6.  [POST BUILD STEPS](#org92cddaf)
        1.  [Glyph Rename Script](#org2bc5fd1)
        2.  [Fix Fsselection](#org8fdb9d2)

This file is formatted for use with [Org-mode](https://en.wikipedia.org/wiki/Org-mode).


<a id="org1788c6c"></a>

# PUBLIC SANS WORKLOG


<a id="org9a19068"></a>

## BASIC INFO

RELEVANT LINKS:
    <https://github.com/google/fonts/pull/1934>
    <https://github.com/uswds/public-sans>

STATUS:
    Fixing PR bot errors

NOTES:

1.  PR Needs to be split in two


<a id="org487908e"></a>

## FONTBAKERY STATUS


<a id="org942d221"></a>

### ROMAN

1.  FAILS 05 **\*\***

    1.  DONE :: check/os2<sub>metrics</sub><sub>match</sub><sub>hhea</sub>
    
        ACTION LOG &#x2013; Fixing this in the source:
        
        1.  Changed typoDescender to -653 from 653 on all masters
        2.  Reordered parameters
    
    2.  DONE :: check/integer<sub>ppem</sub><sub>if</sub><sub>hinted</sub>
    
        ACTION LOG &#x2013; This needs these steps:
            mkdir ttx && ttx -d ttx -s Lemonada-Regular.ttf
            v ttx/Changa-VF.<sub>h</sub><sub>e</sub><sub>a</sub><sub>d.ttx</sub>
            ttx ttx/Changa-VF.ttx
            cp ttx/Changa-VF.ttf Changa-VF.ttf
            fontbakery check-googlefonts -l WARN Changa-VF.ttf &#x2013;ghmarkdown fb.md
    
    3.  DONE :: check/metadata/nameid/copyright
    
        Changed to:
        Copyright 2011 The Lemonada Project Authors (<https://github.com/Gue3bara/Lemonada>)
    
    4.  :: check/production<sub>encoded</sub><sub>glyphs</sub>
    
        Glyph is from Unicode block: Private Use Area &#x2013; U+E000 to U+F8FF
        NBD: Won't fix for now
    
    5.  :: check/metadata/valid<sub>filename</sub><sub>values</sub>
    
        NBD: Won't fix
    
    6.  :: check/canonical<sub>filename</sub>
    
        NBD: Won't fix
    
    7.  :: check/metadata/has<sub>regular</sub>
    
        NBD: Won't fix
    
    8.  :: check/description/max<sub>length</sub>
    
        This should be fixed&#x2026; but maybe make the PR anyway.

2.  WARNS 03 **\*\***

    1.  :: check/points<sub>out</sub><sub>of</sub><sub>bounds</sub>
    
        NBD: Won't fix for now
    
    2.  :: check/production<sub>glyphs</sub><sub>similarity</sub>
    
        NBD: Wont fix for now
    
    3.  :: check/unitsperem<sub>strict</sub>
    
        NBD: Wont fix for now


<a id="org8ed5b39"></a>

### ITALIC


<a id="orgef99eb7"></a>

## TODO S


<a id="org507cd35"></a>

### DONE Close old PR


<a id="org8dbf3f9"></a>

### DONE Make GF-mastering branch


<a id="org61e150d"></a>

### TODO PR Public Sans


<a id="orgbd4fbdd"></a>

### TODO PR Public Sans Italic


<a id="orged65776"></a>

## BUILD HELPERS


<a id="org932f3b0"></a>

### FontBakery


<a id="orgb26ae80"></a>

### Addfont


<a id="org0fd3b81"></a>

### Build Commands


<a id="orga6a23d3"></a>

### Build Info


<a id="orgb4ba37a"></a>

## BUILD STEPS

./BUILD.sh
    #!/bin/sh
    python3 sources/BUILD.py \\
    &#x2013;ttfautohint "-v &#x2013;stem-width-mode=qsq" \\
    &#x2013;googlefonts ~/Google/fonts/ofl/publicsans \\


<a id="org92cddaf"></a>

## POST BUILD STEPS


<a id="org2bc5fd1"></a>

### Glyph Rename Script


<a id="org8fdb9d2"></a>

### Fix Fsselection

gftools fix-fsselection Changa-Regular.ttf &#x2013;autofix

