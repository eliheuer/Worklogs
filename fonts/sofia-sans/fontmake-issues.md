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

