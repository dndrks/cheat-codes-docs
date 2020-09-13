---
layout: page
title: loops
permalink: /docs-loops/
subdoc: true
order: 1
level: 1
---

# navigation

## `E1`
change focus between loop lanes (three banks and the Live buffer)  

<img src="/assets/images/loops_page_nav.gif" style="max-width:35%"/>

*nb. the `s:`tart and `e:`nd times in the top right corner reflect the loop points for the selected lane*

# control

## `K3`
cycle through different sets of controls for the focused loop lane

### **`K3` pad controls**  
- loop points
- rate + slew
- buffer reference + semitone offset

<img src="/assets/images/loops_param_jump.gif" style="max-width:35%"/>

### **`K3` Live buffer controls**  
- loop points
- total length + feedback amount
- mode (looping or 1-shot) + random record probability

<img src="/assets/images/loops_live_params.gif" style="max-width:35%"/>

*nb. the % counter on the second page indicates playhead position in relation to loop length*

### **`K1` + `K3` pad loop**  
- enables / disables looping on the selected bank's current pad
- when you hold K1, you will see an asterisk next to the selected lane

<img src="/assets/images/loops_toggle_loop.gif" style="max-width:35%"/>

*nb. the `L` on the right of the lane reflects that the current pad is looping*

### **`K1` + `K3` Live buffer enable**  
- enables (arrow) / disables (point) recording to the Live buffer
- if in *loop* mode, recording will engage wherever the playhead is located between the loop points
- if in *once* mode, recording will begin at the loop start point

<img src="/assets/images/loops_live_rec.gif" style="max-width:35%"/>

## **`encoders`**
encoder functions depend on the current control set

### **pad loop points**
- `E2`: move start point (coarse, 0.1s)
- `E3`: move end points (coarse, 0.1s)
- `K1 hold` + `E1`: move start and end together (coarse, 0.1s)
- `K1 hold` + `E2`: move start point (fine,0.01s)
- `K1 hold` + `E3`: move end point (fine,0.01s)

<img src="/assets/images/loop_move_points.gif" style="max-width:35%"/>

### **Live buffer loop points**
see `PARAMETERS > loops + buffers > rec loop enc resolution` to choose the resolution of an encoder turn.  
0.1s and 0.01s are absolute time scales, while (1/16, 1/8, 1/4, 1/2, 1 bar) are derived from the current bpm.  
*nb. when switching resolutions, the Live buffer loop window will snap to one unit of the specified resolution.*
- `E2`: move start point (based on `rec loop enc resolution`)
- `E3`: move end points (based on `rec loop enc resolution`)
- `K1 hold` + `E1`: jump loop points together (uniformly distributed, if possible)

if `rec loop enc resolution` is at its default 0.1s, these additional actions are available:
- `K1 hold` + `E2`: move start point (fine,0.01s)
- `K1 hold` + `E3`: move end point (fine,0.01s)

<img src="/assets/images/loops_rec_loop_enc.gif" style="max-width:35%"/>

E1 + K1
loop window: move window
settings: change pad

E2
loop window: move start point for current pad (coarse, 0.1s)
settings: change left setting

E3
loop window: move end point for current pad (coarse, 0.1s)
settings: change right setting

E2 + K1
loop window: move start point for current pad (fine, 0.01s)
settings: change left setting for ALL pads

E3 + K1
loop window: move end point for current pad (fine, 0.01s)
settings: change right setting for ALL pads

Loop:

E1 + K1
loop window: move window uniformly
settings: change Live buffer

E2
loop window: move start point for current buffer (coarse, 0.1s)
settings: change total buffer length (8s, 16s, 32s)

E3
loop window: move end point for current buffer (coarse, 0.1s)
settings: adjust feedback

### pads:

||---|---|---|K1|K2|K3|
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|**E1**| navigate between loop lanes | boop | boop | boop | boop | boop |
|**E2**| boop | boop | boop | boop | boop | boop |
|**E3**| boop | boop | boop | boop | boop | boop |
|**K1**| boop | boop | boop |---|---|---|
|**K2**| boop | boop | boop |---|---|---|
|**K3**| boop | boop | boop |---|---|---|