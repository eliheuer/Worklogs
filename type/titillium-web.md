
# Table of Contents

1.  [TitilliumWeb](#org5250518)
    1.  [BASIC INFO](#org80ca448)
    2.  [RELEVANT LINKS](#org36a0628)
    3.  [WORK STATUS](#org3e17312)
    4.  [FONTBAKERY STATUS](#org0130625)
        1.  [ROMAN](#org2823556)
    5.  [S](#orgee55f14)
        1.  [Close old style PR and open a new style PR.](#org085845c)
    6.  [BUILD STEPS](#org2bb2e37)
        1.  [STEP 1: Run build script](#org67aa420)
    7.  [BUILD HELPERS](#org5c9a9ab)
        1.  [FontBakery](#org21cd304)
        2.  [Addfont](#orgc0e8043)
        3.  [Build Commands](#org40167e9)
        4.  [Build Info](#orgb4b8363)
    8.  [POST BUILD STEPS](#org3cdda58)
        1.  [Glyph Rename Script](#orga3096c0)
        2.  [Fix Fsselection](#orga9fcf3d)



<a id="org5250518"></a>

# TitilliumWeb


<a id="org80ca448"></a>

## BASIC INFO

Arabic/Latin typface.


<a id="org36a0628"></a>

## RELEVANT LINKS

Origin:        <https://github.com/eliheuer/titillium-web-vf>
Upstream:      <https://github.com/eliheuer/titillium-web-vf>
Google Fonts:  <https://fonts.google.com/specimen/Titillium+Web>
Old style PR:  <https://github.com/google/fonts/pull/1806>
New style PR:  None yet


<a id="org3e17312"></a>

## WORK STATUS

Needs a new style PR


<a id="org0130625"></a>

## FONTBAKERY STATUS


<a id="org2823556"></a>

### ROMAN

1.  FAILS 01 **\*\***

    1.  TODO :: check/canonical<sub>filename</sub>
    
        NBD: Won't fix

2.  WARNS 02 **\*\***

    1.  :: check/production<sub>glyphs</sub><sub>similarity</sub>
    
        NBD
    
    2.  :: check/unitsperem<sub>strict</sub>
    
        NBD


<a id="orgee55f14"></a>

## TODO S


<a id="org085845c"></a>

### TODO Close old style PR and open a new style PR.


<a id="org2bb2e37"></a>

## BUILD STEPS


<a id="org67aa420"></a>

### STEP 1: Run build script

./BUILD.sh


<a id="org5c9a9ab"></a>

## BUILD HELPERS


<a id="org21cd304"></a>

### FontBakery


<a id="orgc0e8043"></a>

### Addfont


<a id="org40167e9"></a>

### Build Commands


<a id="orgb4b8363"></a>

### Build Info


<a id="org3cdda58"></a>

## POST BUILD STEPS


<a id="orga3096c0"></a>

### Glyph Rename Script


<a id="orga9fcf3d"></a>

### Fix Fsselection

gftools fix-fsselection Font-Regular.ttf &#x2013;autofix

