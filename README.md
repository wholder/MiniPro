# MiniPro
MiniPro is a command line utility for the [AutoElectric MiniPro TL866CS or TL866A Universal Programmer / Reader](http://www.autoelectric.cn/en/tl866_main.html) that runs on Mac OSX.  It's based on the project https://github.com/vdudouyt/minipro and is provided here as a JetBrains CLion project.  In addition, I've added the ability to read and write to/from Intel Hex ASCII files by adding the suffix ".hex" to the the file name used for reading or writing.

For a good overview of the MiniPro TL866, see this [EEVBlog video](https://www.youtube.com/watch?v=FLG03f_ua5g) and the related [EEVBlog Forum](https://www.youtube.com/redirect?q=http%3A%2F%2Fwww.eevblog.com%2Fforum%2Fblog%2Feevblog-411-minipro-tl866-universal-programmer-review%2F&redir_token=qVo5f3e0YeGbZyTw99Xut424r2l8MTUyMzA2MTk2NkAxNTIyOTc1NTY2&event=video_description&v=FLG03f_ua5g).

Note: you can download just the executable file from https://github.com/wholder/MiniPro/tree/master/cmake-build-debug but you will need to run chmod on the file to make it executable and run it in Terminal:

    >chmod 755 MiniPro.dms
    >MiniPro.dms
    minipro version 0.1     A free and open TL866XX programmer
    Usage: MIniPro.dms [options]
    options:
    	-l		List all supported devices
    	-r <filename>	Read memory
    	-w <filename>	Write memory
    	-e 		Do NOT erase device
    	-u 		Do NOT disable write-protect
    	-P 		Do NOT enable write-protect
    	-v		Do NOT verify after write
    	-p <device>	Specify device (use quotes)
    	-c <type>	Specify memory type (optional)
    			Possible values: code, data, config
    	-i		Use ICSP
    	-I		Use ICSP (without enabling Vcc)
    	-s		Do NOT error on file size mismatch (only a warning)
    	-S		No warning message for file size mismatch (can't combine with -s)
    	-x		Do NOT attempt to read ID (only valid in read mode)
    	-y		Do NOT error on ID mismatch
    	-h		Show help (this text)
