# halcon-calplate
Generates the art for Halcon's stock calibration files and includes pre-generated files if you don't have Halcon.

There is no need for these if you have a normal version of Halcon, you can generate your own files and they don't need to match the standard files. What is important is that you have a matching description file for any calibration plate you generate.  Since you are making you own Halcon will also generate that for you!

These are only useful if you are trying to manufacture plates for people and you don't have Halcon, or purhaps you have some kind of runtime-only environment which is expecting a stock plate and you don't have access to one anymore.

To regenerate the files just cut and paste into a Halcon-XL window and run it. If you don't have Halcon use one of the pre-generated files.  You probably want the pre-generated "fixed" ones anyway and the scripts to correct the files rely on linux tools, so if you only have windows just use the pre-generated ones and don't bother re-creating them as you won't be able to perform the final post-processing steps.

Repo also includes a few sample shell scripts/oneliners to remove the unusual tag that MVTec has on the bottom of the plates that makes them asymmetric (I suspect these are where a label would go) but they rely on linux tools.  The "fixed" directory includes files which have these appendages removed, you probably want these if you are trying to make a high-quality plate.

The scripts also generate DXF files (which is undocumented) that can be converted to a gerber for use in a mask printer (for making the tiny ones).

Run under Halcon-XL, not the normal one, it needs the extra precision for the DXF files.

If you print the pdf's make sure you don't "fit" them to the page size.  It wouldn't be a bad idea to examine the dot sizes with some kind of reticule just to verify that nothing got scaled in the printing process.
