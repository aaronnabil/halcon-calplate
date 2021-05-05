# halcon-calplate
Generates the art for Halcon's stock calibration files.

There is no need for these if you have a normal version of Halcon, you can generate your own files and they don't need to match the standard files. What is important is that you have a matching description file for any calibration plate you generate.  Since you are making you own Halcon will also generate that for you!

These are only useful if you are trying to manufacture plates for people and you don't have Halcon, or purhaps you have some kind of runtime-only environment which is expecting a stock plate and you don't have access to one anymore.

Just cut and paste into a Halcon-XL window and run it.

Directory includes a few sample shell scripts/onliners to remove the unusual tag that MVTec has on the bottom of the plates that makes them asymmetric (I suspect these are where a label would go).  The "fixed" directory includes files which have this removed, you probably want these if you are trying to make a high-quality plate.

The scripts also generate DXF files (which is undocumented) that can be converted to a gerber for use in a mask printer (for making the tiny ones).

Run under Halcon-XL, not the normal one, it needs the extra precision for the DXF files.
