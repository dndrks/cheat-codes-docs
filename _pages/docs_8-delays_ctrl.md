---
layout: page
title: ctl
permalink: /docs-delays_ctl/
subdoc: true
order: 11
level: 2
---

<img src="../assets/images/delays_2ctl-hd.png" class="mw-60" />

## timebase
---

each delay can be set to either of two modes:

- **clocked**: delay length is equal to x number of beats at the current bpm, ranging from 1/4 beat to 16 beats with 98 steps in between
- **free**: delay length is freely definable, ranging from 0 to 30 seconds
  - hold `K1` while adjusting the **free** length to adjust at 1/1000s resolution
  - for best results, keep *fade time* less than or equal to delay length

if both delays have the same timebase, they can form a mono signal -- even a small offset will help create a nice stereo spread.

## rate
---

each delay's rate can be manipulated to add depth.  
rate can range from quarter-speed to 24x. hold `K1` to adjust by hundredths.  
a nice aliasing effect can be achieved by setting a 0.001s timebase and fade and setting rate to fractional values.

## feedback
---

each delay has a feedback setting, which ranges from 0 to 100%.  

when `K1` is held, a *jump* in feedback value is performed:

- if feedback > 0% then *jump* sets to 0%
- if feedback == 0% then *jump* sets to 100%

this creates an opportunity to use the delay as a destructive audio looper!