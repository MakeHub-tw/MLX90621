# MLX90621

MLX90621 code for various platforms

## Use git's `submodule` command to download other repositories

Most of the subdirectories in this repository are selectively cloned from open source projects as submodules. Thank them for their selfless dedication. Use the command below to clone the full repository

    git clone --recursive https://github.com/MakeHub-tw/MLX90621.git

Or alternatively, if you've already cloned this repository. Just `cd` to it and execute the following commands inside:

    git submodule init
    git submodule update

Enjoy!

## What's included

### MLX90621-library for `mbed`

This is the official library from Melexis - https://github.com/melexis/MLX90621-library

The driver inside the repository is designed to work on [mbed](https://www.mbed.com/), but it seems not so hard to port it to other platforms. 

### Arduino

I've tested https://github.com/robinvanemden/MLX90621_Arduino_Processing and it seems to work well.

It seems to be a good idea to port the official library on Arduino as well.

### Raspberry Pi

Inside this subfolder, I've included https://github.com/rod0/thermomin

It works, but the values returned seem to be shifted. It's also possible to port the official algorithm to replace the original one.

By the way, this repository makes use of software I2C to avoid clock stretching, I don't know whether this matters.