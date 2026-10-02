# 31.7.1

## Major
 -

## Features
 -

## Performance
 -

## Fixes
 - A packet that fails to decode no longer aborts the whole analysis. The bad packet is skipped with a warning and the rest of the file is still read, so one damaged frame in a long recording can't throw away the entire result.
 - Analysis now drains the decoder at the end of a stream, instead of stopping a frame or two short of it.
 - An analysis taken over skipped packets is no longer written to the cache, so holes can't be served back as real silence on later runs.
 - `levels` exits non-zero when it had to skip packets. The values it did read are still printed; the exit status is how a caller learns the reading is incomplete.
 - Progress output goes to stderr instead of stdout, where it could land in the middle of `levels`, `waveform`, and `--export v1 -o -` data.

# Misc.
 -
