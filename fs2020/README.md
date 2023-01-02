# Index

#### `bin/avionics-stream`

This script uses `v4l2` to setup two windows (using `ffplay`) that show the G1000 PFD and MFD respectively.
The windows need to be placed on the desktop in a specific location as to appear below the G1000 panels as rendered by Air Manager.
The G1000 screens are rendered by FS2020 and streamed via a capture card to the Linux machine running Air Manager.
`ffmpeg` is then used to create two video streams `/dev/video4` and `/dev/video7` for the PFD and MFD respectively from the capture card output on `/dev/video0`.
