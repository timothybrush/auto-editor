# 31.6.1

## Major
 -

## Features
 - `info --json` now reports `decodable` for every audio stream: whether this build has a decoder for it.

## Performance
 -

## Fixes
 - Skip undecodable audio streams when rendering a `.v3` timeline too, not only when building one. A timeline written elsewhere no longer fails on the `apac` track in iPhone Spatial Audio recordings.

# Misc.
 -
