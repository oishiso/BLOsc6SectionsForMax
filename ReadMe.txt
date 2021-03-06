The mechanism of this object is explained in “Additive synthesis with band-limited oscillator sections”, Peter Pabon & So Oishi, ICMC 2016.
http://www.icmc2016.com/proceedings.pdf#page=31


============================

blosc6sections~.mxo
(Band-limited oscillator with 6 sections)

This object allows users to draw arbitrary spectrum by moving 6 breakpoints. Less control, but more CPU-friendly than “blosc9sections~”.

See demo video at:
http://sooishi.com/engineering/

============================

Requirements:
Object “blosc6sections~.mxo” only works in Max 6.1 or higher. It is not compatible with earlier versions of Max.

============================

How to install:
- Start Max and add the folder “BLOsc6SectionsForMax” to your file search path.
(From Menu “Options” > “File Preferences” > “+” button at lower left corner of the window)
- Open “blosc6sections~ demo.maxpat” to play demo

============================

Contents of folder “BLOscFor6SectionsForMax”:

blosc6sections~ demo.maxpat - Demo Max patch

blosc6sections~.mxo - Max object

============================

Instruction for using object:

The object has both real (cosine-sum) output and imaginary (sine-sum) output from two outlets. In the demo patch, you can see the waveform from both outlets.

Amplitude normalization function is implemented in “blosc6sections~” object, thus output amplitude keeps same regardless of its parametric values. Amplitude normalization is done by fixing the maximum displacement value of real output to 1, and this means the maximum displacement value of imaginary output is less than 1. 


Object “blosc6sections~” has 1 argument: 
"Fundamental Frequency”

Object “blosc6sections~” has 16 input parameters from inlets:
(From left inlet)
"Fundamental Frequency"
"Hz at Break Point 0"
"dB at Break Point 0"
"Hz at Break Point 1"
"dB at Break Point 1"
"Hz at Break Point 2"
"dB at Break Point 2"
"Hz at Break Point 3"
"dB at Break Point 3"
"Hz at Break Point 4"
"dB at Break Point 4"
"Hz at Break Point 5"
"dB at Break Point 5"
"Hz at Break Point 6"
"dB at Break Point 6"
"Even to Odd Harmonics Amp Ratio"

============================

About the demo MAX patch:

- Presentation Mode
The patch opens in presentation mode. 
To quit presentation mode, “View” > “Presentation”, or Option+Command+E.
To change the default opening mode, go “View” > “Patcher Inspector” > Uncheck “Open in Presentation”.

- Amplitude Envelope
Amplitude envelope can be on/off.
When in “With Env” mode, it can be repeatedly triggered by checking “repeat play“ box. When “repeat play” is off, one-shot trigger can be done by clicking “play” button.


============================
License
Copyright (c) 2017 So Oishi and Peter Pabon. All rights reserved.
This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version.


============================
Author
So Oishi<oishiso@gmail.com>
sooishi.com