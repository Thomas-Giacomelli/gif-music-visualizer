gif-music-visualizer
====================
Visualization of live audio using gifs. This is based on Scott W Harden's ["Realtime FFT Audio Visualization with Python"](http://www.swharden.com/blog/2013-05-09-realtime-fft-audio-visualization-with-python/).

Prepare gif
-----------
Use ImageMagick:
`convert -coalesce image.gif image.png`

Create a directory in the `frames` subdirectory and copy the image frames into it.

Dependencies
------------
* pygame
* scipy
* numpy

Debian:
`apt-get install python-pygame python-scipy python-numpy python-pyaudio`

Usage
-----
Play some audio and run visualizer.py. Press F11 to toggle full-screen mode. Use Escape to exit.

I had to use pavucontrol (PulseAudio Volume Control `apt-get install pavucontrol`) to select "Analog Stereo Output" instead of "Analog Stereo Duplex" (Configuration tab). If you want to use an external input device (like a microphone) use "Analog Stereo Input".
