# shfts
2-voice shift registers for norns &amp; grid

## details
~~~
-- shfts
-- 2 voice double binary shift register
-- + midi + dual quantizers
--
-- enc1: bpm
-- enc2: voice 1 pitch offset
-- enc3: voice 2 pitch offset
-- key2: start/stop voice 1
-- key3: start/stop voice 2
-- 
-- Midi device/channel output can be set per voice in params
-- 
-- GRID UI
-- 2 completely symmetrical voices, 8 columns each
-- row 1 - pitch register bit display
-- row 2 - trigger register bit display
-- row 3 - loop length (per voice)
-- row 4 - clock division (per voice)
-- row 5 - pitch change prob (first 4) pitch octave range (last 4)
-- row 6 - trigger change prob (first 4) trigger bias (last 4)
-- row 7 - quantizer presets - hold a button and press keys from row 1-6; 
-- layout is perfect fourths vertical, chromatic scale horizontal
-- row 8 - kind of a mess right now, will have start/stop, write/shift manual controls (i think)
~~~

## TODO (roughly in order)
- document grid layout (in the meantime the norns screen is pretty descriptive)
- test 2-channel quantizer
- save quantizer presets
- crow!
- consider giving trigger bias a dedicated row on the grid and moving pitch range to a param
- note-off and note duration mostly work, but there are some edge cases with a starting/stopping midi clock
- rethink clocking generally, allow for unclocked manual stepping (crow gate inputs?)

## license
CC Attribution-NonCommercial-NoDerivatives 4.0 for now, since I am rushing this out a bit ahead of schedule and haven't had a chance to think about rights much.  If you want to use this code, get in touch - if it's legit I'm happy to grant a more permissive license as needed.