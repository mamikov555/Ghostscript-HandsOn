# Ghostscript-HandsOn

Ghostscript consists of a PostScript interpreter layer, and a graphics library. The graphics library is shared with all the other products in the Ghostscript family, so all of these technologies are sometimes referred to as Ghostscript, rather than the more correct GhostPDL.

# Checking if the specific **PDF** file is passing validation. 
The command line option '-sDEVICE=device' selects which output device Ghostscript should use. If this option isn’t given the default device (usually a display device) is used

```bash
gs -dNOPAUSE -dBATCH -sDEVICE=nullpage filename.pdf
```

# Converting a PDF file to TIFF file.
Using Ghostscript command to convert manually PDF file to TIFF file, render it with 200 dpi. With the option _-sDEVICE=tiffgray_, we are specifying the output tiff file to be 8-bit gray.

_-dNOPLATFONTS_ - disables the use of fonts supplied by the underlying platform

```bash
gs -r200 -dBATCH -sDEVICE=tiffgray -dNOPAUSE -dSAFER -dPDFSTOPONERROR -dNOPLATFONTS -sOutputFile=output.tiff filename.pdf
```
