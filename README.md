# Intellectual Bottle Recycle Bin
Group Member: Shimei Qiu, Yuni Xie, and Yeting Bao.

Create an intellectual bottle recycle bin for the recycling department near your place. Once you drop a bottle into the special bin, the screen besides it will show its material. 
We use the acoustic sensing technology to collect the echoes when a bottle is drops into a box, and apply machine learning method to recognize the sound made from which material.

## Photon Connection
[Adafruit 1713] :

A0 - Output

GND - GND

VCC - 3V3

## Code
1. microphone.ino

Photon code for recording audio.

2. audioserver.js

Before using, install the npm package "wav" and "speaker":
```
npm install wav
npm install speaker
```

Then to build a local server for receiving audio and play it after transition:
```
node audioserver.js
```

3. visualization folder

open.html: The web page to start the recording process on photon.

predict.html: The web page to analyze the audio and visualize the prediction.

## Resource
Photon Audio Example Code: https://github.com/rickkas7/photonAudio
