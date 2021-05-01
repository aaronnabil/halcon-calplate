# halcon-calplate
Generates the art for Halcon's stock calibration files

This script generates art files for Halcon calibration plates that correspond to the standard calibration files.

Cut and paste into a Halcon-XL window and run it.

Directory includes a few sample shell scripts/onliners to remove the unusual tag the MVTec has on the bottom of the plates that makes them asymmetric (I suspect these are where a label would go).

These also generate DXF files (which is undocumented) that can be converted to a gerber for use in a mask printer (for making the tiny ones).

Run under Halcon-XL, not the normal one, it needs the extra precision.
