# GPS-Sim-HackRF

Inhere you will find the GnuRadioCompanion.gru for the GPS Static location menu and replay.
Make sure to 
## Table of Contents
- [Installation](#installation)
- [GPS Vector Generation](#gps vector generation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Install the GnuRadioCompanion at https://wiki.gnuradio.org/index.php/InstallingGR
2. import the GPSsimulator.grc from this repository
3. Make sure to change your HackerRF One USB id-number as mentioned in the youtube video: https://www.youtube.com/watch?v=gBBOOR24J3w&ab_channel=YarivShavit
4. Make sure to change the directories of the vectors in the block diagram (mentioned in the video) (see GPS Vector Generation)
5. Once set, it should be working by REPLAY from the GNURadio Menu

## GPS Vector Generation
Becaus e the vector were to big, you will have to create them yourself.
1. download the gps-sdr-sim.exe into a new Folder
2. Via the File explorer type "cmd" to get to the windows command line.
3. type gps-sdr-sim -d 300 -b 8 -e brdc0260.24n -l <Lat,Lon,Hgt> // chose for lon lat the town of your interess.
4. Press enter, you should see a progress and a vector in the same folder being created, named gpssim.bin. Rename it to the location of interess.
5. Do this for other locations
6. you can see the command gps-sdr-sim.tx for examples.

## Usage
You can replay the GPS location to any GPS receiver cunducted or wireless.
by changing the RF Gain you can play with the output TX power of the HackRFOne.
```bash

