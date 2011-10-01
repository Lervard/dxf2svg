# 01 Oct 2011

I (Nick Markwell, aka @duckinator) have apparently taken over this after it being dead for 5 years.
I have gotten it to compile again, and I'm starting to clean up the code a bit.
I have not actually tested it.

All information from before October 01, 2011 is by Matt Squires. I have, however, reformatted it all.

# 27 Aug 2005

Fixed a fair number of bugs, and broken conversions. LWPOLYLINE works now, text rotation is ok but needs multiple transfomations to get it right, can read broken dxf files (w/o dxf EOF information)


# 26 Aug 2005

To use:
I have only gotten this to work with Inkscape under linux (debian sarge).  But the converter works from the commandline if you want to test it otherwise.

1.  Run make and copy dxf2svg to somewhere that is looked at by the PATH variable.  Or add the current directory to your path
2.  Copy the dxf_import.inx to ../Inkscape/share/extensions
3.  Run Inkscape
4.  Click on open or import and the dxf option should be there

I have compiled and then succesfully converted dxf files to svg files with the following setups

WinXP Pro, Cygwin, g++ 3.3.3
Debian Sarge, AMD x86_64, g++ 4.0.2
RedHat(?), x86(?), g++ 3.2.3

I have weakly tried and failed to compile using 
Borland's free compiler bcc32
MinGW

What is supported:
polylines, lines, arc, circles, blocks, text, and a little linetypes

currently not supported but I hope will be in the near future (probably after Sept 05)
layers, colors, trace, splines, dimentions

If you don't have dxf files of your own, but would like to easily test some I would suggest a few places...

www.newfocus.com -- look under optomechanics.  There are a variety of mounts and such that are posted in dxf and pdf
www.thorlabs.com -- dido what I said about newfocus

Free CAD programs:
Windows -- A free and not too bad CAD program for windows is CadStd Lite.  It exports to dxf and has a variety of samples.
Windows/Linux -- QCad is ok.  It has a lot of nice features but when I used it a year ago it would import dxf files but then you couldn't edit what was imported.  It is free but with a time limit.  My experience is that it can be a little annoying.  Because of that and others comments I didn't use their libraries for dxf reading.


Matt Squires
squiresm@colorado.edu

