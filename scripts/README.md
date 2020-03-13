# Scripts

This directory contains a variety of helpful utility scripts for getting your Troopduino up and running.

## copy-to-sdcard

This shell script provides an easy method to properly copy the files from the `sdcard` directory to your Troopduino SD card.
To properly format the SD card, run the following commands from a terminal (OSX):

- `sudo diskutil list`

  This will display the all the volumes attached to your machine.  Search for the SD card volume, which can most likely be found
  by the volume size (i.e. `/dev/disk2`).

- `sudo diskutil eraseDisk FAT32 <volume_name> MBRFormat /dev/disk2`

  This will reformat and rename the SD card.  Replace `<volume_name>` with whatever you like.
  
- `./copy-to-sdcard ../sdcard <volume_name>`

  From the `Troopduino-Code/scripts` directory, run the above command, replacing `<volume_name` with the name you selected
  when formatting the SD card above.
  
### Background

Troopduino requires all sound files to be in the root with filenames in the this sequential format `####.wav`, starting with
`0001.wav`, which corresponds to track index 1 in the code.  Additionally, the files timestamps must be in increasing order as
well, which the copy script takes care of.
