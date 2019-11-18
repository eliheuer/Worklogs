# Worklog: Chomsky
```
Last Updated:       Tuesday November 5th 2019
Progress Estimate:  20%
```

## Basic Info
A font in the style of the New York Times masthead

## Project Links
| Relevant Links             | URLs                                                                                     |
| ------------------         | :--------------------------------------------------------------------------------------- |
| Working Git Repository     | [https://github.com/eliheuer/chomsky](https://github.com/eliheuer/chomsky)               |
| Upstream Git Repository    | [https://github.com/ctrlcctrlv/chomsky](https://github.com/ctrlcctrlv/chomsky)           |
| Google Fonts Page          | [None Yet](https://fonts.google.com)                                                     |
| Google/fonts Pull Request  | [None Yet](https://github.com/google/fonts/pull/aaaa)                                    |

## Work Status
- [ ] Merged to [google/fonts](https://github.com/google/fonts)
- [ ] Changes requested on [github](https://github.com/google/fonts/pull/aaaa)

## TODO List
- [ ] Clean up curve pointcount
- [ ] Check char set
- [ ] Update char set to GL-Core
- [x] Add a TODO list

## Worklog
### Thursday November 7th, 2019
```
making a new branch: opsz-update
```

### Tuesday November 5th, 2019
```
More basic repo review
```

## Notes
```
MERGE TARGET
------------
Character Set: Google Latin Core
Variations:    opsz
```
```
No RFN
```

```
from Foundation import NSPoint
layer = Glyphs.font.selectedLayers[0] # current layer

# make anchor at (0,0)
layer.anchors['top'] = GSAnchor()

# set position
layer.anchors['top'].position = NSPoint(425, 748)

# read position
print(layer.anchors['top'].position.x, layer.anchors['top'].position.y)
```
