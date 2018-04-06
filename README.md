# MiniPro
MiniPro is a command line utility for the MiniPro TL866CS or TL866A device Programmer / Reader that runs on Mac OSX.  It's based on the project https://github.com/vdudouyt/minipro and is provided here as a JetBrains CLion project.  In addition, I've added the ability to read and write to/from Intel Hex ASCII files by adding the suffix ".hex" to the the file name used for reading or writing.

Note: you can download just the executable file from https://github.com/wholder/MiniPro/tree/master/cmake-build-debug but you will need to run chmod on the file to make it executable and run it in Terminal:

    >chmod 755 MiniPro.dms
    >MiniPro.dms
