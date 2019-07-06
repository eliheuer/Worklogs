# Worklog: Changa VF Mastering

Last Updated: Mon Jul 3, 2019

- [x] First PR
- [x] Pending change request
- [ ] Waiting for review
- [ ] Reviewer says OK
- [ ] Merged

## Table of Contents

* [Basic Info](#basic-info)
* [Project Link](#project-links)
* [Work Status](#work-status)
* [FontBakery Status](#fontbakery-status)
* [Build Steps](#build-steps)
* [Post Build Steps](#post-build-steps)
* [Notes](#notes)
* [Worklog](#Worklog)

## Basic Info

Arabic/Latin Typeface

## Project Links

| Relevant Links | URLs                                                                                   |
| -------------- | :------------------------------------------------------------------------------------- |
| Origin repo    | [https://github.com/eliheuer/changa-vf](https://github.com/eliheuer/changa-vf)         |
| Upstream repo  | [https://github.com/etunni/Changa](https://github.com/etunni/Changa)                   |
| Google Fonts   | [https://fonts.google.com/specimen/Changa](https://fonts.google.com/specimen/Changa)   |
| Pull request   | [https://github.com/google/fonts/pull/1949](https://github.com/google/fonts/pull/1949) |

## Work Status

- [x] New style PR
- [x] PR spec updated
- [ ] Update upstream source repo
- [ ] Pending change request

## FontBakery Status

Nothing here.

## Build Steps

Run Build Script
```
./BUILD.sh
```

## Post Build Steps

```
gftools fix-fsselection Font-Regular.ttf --autofix
```

## Notes

Nothing here.

## Worklog

#### Wed July 3, 2019

- [ ] Look into merging upstream.
    - Compare Gabber's fork and mine
    - Start a new branch for a pr back to upstream
- [ ] Update PR to new spec
    - Foobar
