## Color

### Tag: `10bit`

Parse: `yuv420p10le` (`10le`)

From sample probe snippet:

`Stream #0:0: Video: hevc (Main 10), yuv420p10le(tv), 1920x1040, SAR 1:1 DAR 24:13, 23.98 fps, 23.98 tbr, 1k tbn (default)`

---

### Tag: `HDR`

Parse: `bt2020nc/bt2020/smpte2084` (`bt2020`)

From sample probe snippet:

`Stream #0:0: Video: hevc (Main 10), yuv420p10le(tv, bt2020nc/bt2020/smpte2084), 3840x2076, SAR 1:1 DAR 320:173, 23.98 fps, 23.98 tbr, 1k tbn (default)`

---

### Tag: `Dolby Vision`

Parse: `DOVI configuration record: version: 1.0, profile: 8, level: 6, rpu flag: 1, el flag: 0, bl flag: 1, compatibility id: 1`

From sample probe snippet:

```
Stream #0:0(eng): Video: hevc (Main 10), yuv420p10le(tv, bt2020nc/bt2020/smpte2084), 3840x2160 [SAR 1:1 DAR 16:9], 23.98 fps, 23.98 tbr, 1k tbn (default) (original)
    Metadata:
      BPS             : 15015420
      DURATION        : 01:23:05.981000000
      NUMBER_OF_FRAMES: 119544
      NUMBER_OF_BYTES : 9358324934
      _STATISTICS_WRITING_APP: mkvmerge v73.0.0 ('25 or 6 to 4') 64-bit
      _STATISTICS_TAGS: BPS DURATION NUMBER_OF_FRAMES NUMBER_OF_BYTES
    Side data:
      DOVI configuration record: version: 1.0, profile: 8, level: 6, rpu flag: 1, el flag: 0, bl flag: 1, compatibility id: 1
  Stream #0:1(eng): Audio: eac3, 48000 Hz, 5.1(side), fltp, 192 kb/s (default) (original)
    Metadata: ...
```

Notes: Likely always requires 10bit color (`10le`) with high dynamic range (`bt2020`).
