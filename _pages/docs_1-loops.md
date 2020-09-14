---
layout: page
title: loops
permalink: /docs-loops/
subdoc: true
order: 1
level: 1
---

cheat codes features three banks (a, b, c) of 16 pads (a1-a16, etc).  
each pad can have its own *totally unique* settings for loop points, speed + direction, audio buffer, panning, filtering, etc.  
the `[loops]` page is where you define these settings.

# navigation

<!-- ## `E1` -->

there are four loop lanes on the `[loops]` page; one for each bank and one for the Live buffers.  

`E1` changes focus between them:

<img src="cheat-codes-docscheat-codes-docs/assets/images/loops_page_nav.gif" style="max-width:35%"/>

*nb. the `s:`tart and `e:`nd times in the top right corner reflect the loop points for the selected lane*

# controls

## Live buffers

cheat codes has three Live buffers to record into, which can be customized in a number of ways.

### Live buffer controls

navigate down to the Live loop lane and press `K3` to cycle between:

- loop points (default view)
- total length + feedback amount
- mode (looping or 1-shot) + random record probability

<img src="cheat-codes-docs/assets/images/loops_live_params.gif" style="max-width:35%"/>

*nb. the % counter on the second page indicates playhead position in relation to loop length*

### recording into the Live buffer

with the Live loop lane selected, hold `K1` and press `K3` to toggle recording to the Live buffer on/off.

- if in *loop* mode, recording will engage wherever the playhead is located between the loop points
- if in *once* mode, recording will begin at the loop start point

<img src="cheat-codes-docs/assets/images/loops_live_rec.gif" style="max-width:35%"/>

### Live buffer loop points
see `PARAMETERS > loops + buffers > rec loop enc resolution` to choose the resolution of an encoder turn.  
0.1s and 0.01s are absolute time scales, while (1/16, 1/8, 1/4, 1/2, 1 bar) are derived from the current bpm.  
*nb. when switching resolutions, the Live buffer loop window will snap to one unit of the specified resolution.*
- `E2`: move start point (based on `rec loop enc resolution`)
- `E3`: move end points (based on `rec loop enc resolution`)
- `K1 hold` + `E1`: jump loop points together (uniformly distributed, if possible)

if `rec loop enc resolution` is at its default 0.1s, these additional actions are available:
- `K1 hold` + `E2`: move start point (fine,0.01s)
- `K1 hold` + `E3`: move end point (fine,0.01s)

<img src="cheat-codes-docs/assets/images/loops_rec_loop_enc.gif" style="max-width:35%"/>

### change buffer

## what about pre-recorded samples?

in the `PARAMS`, navigate to 

### pad controls

tap `K3` on any bank's loop lane to switch between these sets of control for the current pad:

- loop points
- rate + slew
- buffer reference + semitone offset

<img src="cheat-codes-docs/assets/images/loops_param_jump.gif" style="max-width:35%"/>

### loop a pad

to get a pad looping without a grid or MIDI keyboard, hold `K1` and press `K3`.  
the `L` on the right of the lane refelcts that the current pad is looping.

<img src="cheat-codes-docs/assets/images/loops_toggle_loop.gif" style="max-width:35%"/>

*nb. when you hold K1, you will see an asterisk next to the selected lane*

### loop points

- `E2`: move start point (coarse, 0.1s)
- `E3`: move end points (coarse, 0.1s)
- `K1 hold` + `E1`: move start and end together (coarse, 0.1s)
- `K1 hold` + `E2`: move start point (fine,0.01s)
- `K1 hold` + `E3`: move end point (fine,0.01s)

<img src="cheat-codes-docs/assets/images/loop_move_points.gif" style="max-width:35%"/>

### rate + slew

*rate* determines the speed and direction of pad playback.  
*slew* determines how many seconds it will take to get to the specified rate.

- `E2`: change rate for the current pad
- `E3`: change slew for the current pad
- `K1 hold` + `E2`: change rate for *all* pads to the value of the current pad
- `K1 hold` + `E3`: change slew for *all* pads to the value of the current pad

NEED GIF

### buffer reference + semitone offset

each pad can be individually set to reference any of the three Live buffers or three pre-recorded Clip buffers.

##### change pad


### **`K3` Live buffer controls:**  
- loop points
- total length + feedback amount
- mode (looping or 1-shot) + random record probability

<img src="cheat-codes-docs/assets/images/loops_live_params.gif" style="max-width:35%"/>

*nb. the % counter on the second page indicates playhead position in relation to loop length*

### **`K1` + `K3` loop pad**  
- enables / disables looping on the selected bank's current pad
- when you hold K1, you will see an asterisk next to the selected lane

<img src="cheat-codes-docs/assets/images/loops_toggle_loop.gif" style="max-width:35%"/>

*nb. the `L` on the right of the lane reflects that the current pad is looping*

### **`K1` + `K3` enable Live buffer**  
- enables (arrow) / disables (point) recording to the Live buffer
- if in *loop* mode, recording will engage wherever the playhead is located between the loop points
- if in *once* mode, recording will begin at the loop start point

<img src="cheat-codes-docs/assets/images/loops_live_rec.gif" style="max-width:35%"/>

# keys

## `K3`
cycle through different sets of controls for the focused loop lane

### **`K3` pad controls:**  
- loop points
- rate + slew
- buffer reference + semitone offset

<img src="cheat-codes-docs/assets/images/loops_param_jump.gif" style="max-width:35%"/>

### **`K3` Live buffer controls:**  
- loop points
- total length + feedback amount
- mode (looping or 1-shot) + random record probability

<img src="cheat-codes-docs/assets/images/loops_live_params.gif" style="max-width:35%"/>

*nb. the % counter on the second page indicates playhead position in relation to loop length*

### **`K1` + `K3` loop pad**  
- enables / disables looping on the selected bank's current pad
- when you hold K1, you will see an asterisk next to the selected lane

<img src="cheat-codes-docs/assets/images/loops_toggle_loop.gif" style="max-width:35%"/>

*nb. the `L` on the right of the lane reflects that the current pad is looping*

### **`K1` + `K3` enable Live buffer**  
- enables (arrow) / disables (point) recording to the Live buffer
- if in *loop* mode, recording will engage wherever the playhead is located between the loop points
- if in *once* mode, recording will begin at the loop start point

<img src="cheat-codes-docs/assets/images/loops_live_rec.gif" style="max-width:35%"/>

## **`encoders`**
encoder functions depend on the current control set

### **pad loop points**
- `E2`: move start point (coarse, 0.1s)
- `E3`: move end points (coarse, 0.1s)
- `K1 hold` + `E1`: move start and end together (coarse, 0.1s)
- `K1 hold` + `E2`: move start point (fine,0.01s)
- `K1 hold` + `E3`: move end point (fine,0.01s)

<img src="cheat-codes-docs/assets/images/loop_move_points.gif" style="max-width:35%"/>

### **change pad**

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

<img src="cheat-codes-docs/assets/images/loops_rec_loop_enc.gif" style="max-width:35%"/>

### **change buffer**

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