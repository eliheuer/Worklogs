# Worklog: Sofia Sans

Last Updated: Tue Aug 28th

## Table of Contents

* [Basic Info](#basic-info)
* [Project Links](#project-links)
* [Work Status](#work-status)
* [Worklog](#Worklog)
* [FontBakery Status](#fontbakery-status)
* [Notes](#notes)

## Basic Info

Latin Typeface

## Proving some issueject Links

| Relevant Links | URLs                                                                                   |
| -------------- | :------------------------------------------------------------------------------------- |
| Origin repo    | [https://github.com/lettersoup/Sofia-Sans](https://github.com/lettersoup/Sofia-Sans)   |
| Forked repo    | [https://github.com/eliheuer/Sofia-Sans](https://github.com/eliheuer/Sofia-Sans)       |
| Google Fonts   | [Nothing yet](https://fonts.google.com)                                                |
| Pull request   | [Nothing yet](https://github.com/google/fonts/pull)                                    |

## Work Status

- [x] Fixing error: Can't find base (neutral) master in DesignSpace document
- [x] Working on a build script

## Worklog

#### Wed Aug 28, 2019

- Helpful Links
    - https://forum.glyphsapp.com/t/avar-axis-mappings/12425/8
    - https://forum.glyphsapp.com/t/generating-an-avar-table/9337/3
    - https://docs.microsoft.com/en-us/typography/opentype/spec/avar
    - https://dev.to/maxwell_dev/the-git-rebase-introduction-i-wish-id-had

#### Wed Aug 7, 2019

- Helpful links:
    - https://github.com/fonttools/fonttools/issues/1570
    - https://github.com/thundernixon/Encode-Sans/blob/master/sources/scripts/helpers/fix-designspace.py
    - https://github.com/thundernixon/Encode-Sans/tree/master/docs/01-morphing-non-rect-designspace

#### Wed Aug 7, 2019

- [x] Yak shaving.

#### Tue Aug 6, 2019

- [ ] Fixing error: Can't find base (neutral) master in DesignSpace document
- Note from group chat:
    - when you define an axis in a designspace, you say min, max, default
    - the "default" must be the value of that axis on one of the sources. E.g. if you set the wght default to 400, you must have a source that is wght=400
    - so, often if you have light and bold masters, you'll need to set the default to be either light or bold. That is the basic set of glyf coordinates, and then the other sources are used for gvar deltas (as far as i understand it – I may not be 100% technically perfect on that description)
    - yeah, eli, my suggestion is to just make the axis default the same as values in the masters. It may mean that the default instance of the font is light or heavy, but that's better than inserting a whole extra master that isn't needed
    - Only have masters where you need them for the design to work. Set the axis default as light or bold – whichever would be less of a problem if someone came across the font in legacy software. Almost all users will see 400 weight, 100 width anyway, as that is the software default that will be rendered by the browser.
    - Relevant issue: https://github.com/googlefonts/fontmake/issues/566
    - Relevant discussion: https://twitter.com/ArrowType/status/1157396110505381889
    - SN

#### Thu July 25, 2019

- [ ] Trying to get everything building with Fontmake
    - [ ] Getting a fontmake error:
      `RecursionError: maximum recursion depth exceeded`
      This issue has been discussed here:
      https://github.com/googlefonts/glyphsLib/issues/375
    - [x] The file names use `CYRILLIC CAPITAL LETTER EM U+041C`
      changed to `LATIN CAPITAL LETTER M U+004D`

## FontBakery Status

Nothing here.

## Notes

# Fontmake issues

New error: cu2qu.errors.IncompatibleFontsError: fonts contains incompatible glyphs: 'blackLargeCircle', 'largeCircle'
blackLargeCircle was noninterp, fixed it in temp.

Ok maybe I should fix the problem glyphs?

Sofia_Sans_vf has junk taken out(zhe, ka), but is otherwise clean.

Fixing infinate recurion issue:

Python debug code: /Py/emode/defcon/Lib/defcon/objects/glyph.py
```python
    def _set_name(self, value):
        oldName = self._name
        if oldName != value:
            self.postNotification(notification="Glyph.NameWillChange", data=dict(oldValue=oldName, newValue=value))
            self._name = value
            self.postNotification(notification="Glyph.NameChanged", data=dict(oldValue=oldName, newValue=value))
            self.dirty = True
        print("DEBUG (value):", value)
```

```
Problem glyphs:

DEBUG (value): zhe-cy
DEBUG (value): ka-cy
```

### Notes on issues: 
https://github.com/thundernixon/Encode-Sans/tree/master/docs/01-morphing-non-rect-designspace

### Load from Gist
font("../../../Type/forks/Sofia-Sans/sources/variable_ttf/NewFont-VF.ttf")


Nothing here.
