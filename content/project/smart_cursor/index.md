---
title: Smart Cursor
date: 2026-05-18
# external_link: https://github.com/pytorch/pytorch
tags:
  - Markdown
index: false
---

Using YOLOv26 + PyQt to build system-wide target facilitation techniques. Credits: Xinqi Tang, Eva-Ly Jerome, Julien Gori.
Built on [TargetFinder](https://jgori-ouistiti.github.io/academic/project/targetfinder/)




### Bubble cursor
Bubble Cursor is an area cursor, whose area grows until reaching the closest target. This essentially makes targets larger. 
Original Bubble Cursor [paper](https://dl.acm.org/doi/abs/10.1145/1054972.1055012).
![Bubble Cursor demo](bubblecursor.gif)

### Dynaspot
Dynaspot is an area cursor whose area grows depending on the instantaneous speed, essentially it is a Bubble Cursor where the area is modulated by speed. The motivation behind this technique is that more precise selection requires slowing down. Original Dynaspot [paper](https://dl.acm.org/doi/pdf/10.1145/1518701.1518911)
![Dynaspot demo](dynaspot.gif)


### Ninjacursor
NinjaCursor is a technique where one moves not a single cursor but an array of cursor. The actual cursor is selected with gaze. The idea is to first aim "with the eyes", and perform finer movements with the mouse.
https://dl.acm.org/doi/pdf/10.1145/1357054.1357201
![Ninjacursors demo](ninjacursors.gif)


### Semantic Pointing
Semantic Pointing is a technique which locally dissociates the mapping between (physical) mouse movements and (virtual) cursor movements. Concretely, this can make targets look sticky or on the contrary, repulsive
![Semantic Pointing demo](semanticpointing.gif)


<!--more-->
