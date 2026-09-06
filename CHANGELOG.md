# 31.6.0

## Major
 -

## Features
 - Add the `tone` audio generator: `add:tone:note[:waveform]` lays a MIDI-pitched sine, saw, square, or triangle wave on its own audio layer.
 - `add:` now brings every stream the source holds, so `add:pip.mp4` adds sound along with the picture and `add:music.mp3` adds background music with no video stream.
 - `drawbox` can now be used as a generator: `add:drawbox:...` paints the box on its own overlay layer instead of onto the picture.

## Performance
 -

## Fixes
 - Skip audio streams no decoder can read, like some tracks in iPhone Spatial Audio recordings.
 - Name the codec when a decoder can't be found.

# Misc.
 - Update the bundled x265 to 4.3 and libvpx to 1.17.0.
