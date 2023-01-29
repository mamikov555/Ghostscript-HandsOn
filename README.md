# Ghostscript-HandsOn

Ghostscript consists of a PostScript interpreter layer, and a graphics library. The graphics library is shared with all the other products in the Ghostscript family, so all of these technologies are sometimes referred to as Ghostscript, rather than the more correct GhostPDL.

# Checking if the specific **PDF** file is passing validation. 
The command line option '-sDEVICE=device' selects which output device Ghostscript should use. If this option isn’t given the default device (usually a display device) is used

```
gs -dNOPAUSE -dBATCH -sDEVICE=nullpage **filename.pdf**
```