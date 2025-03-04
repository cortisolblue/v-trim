# v-trim
A bash script that interfaces with ffmpeg to make it easier to trim videos.

## Purpose
ffmpeg is a powerful tool but I found it difficult to memorize the commands used to trim videos at desired timestamps. I took all the flags that ffpmeg takes to accurately trim videos without losing video quality and utilized them into a bash script, simplifying the syntax required to trim videos.

## Installation
You can copy the raw file into a text file and make it executable with ```chmod +x``` or git clone the repo and make the script executable

## Usage
```v-trim -t HH:MM:SS-HH:MM:SS {INPUT_FILE}```

where the first HH:MM:SS is the starting timestamp and the second HH:MM:SS is the ending timestamp of the video

## Limitations
I originally created this script for a specific project which only required mp4 videos so for now the script will automatically convert your video to mp4 format.
I'll look into adding more functionality to expand the output format options, but in the meantime you can open up the script and look for all of the variables and lines where the output file is written as '.mp4' and change the format manually to your liking. 

## Bonus
v-trim ```-rt``` HH:MM::SS-HH:MM:SS
The -r flag can be used to automatically resize video to 1920x1080@30fps. Again this is a limited feature that I plan on expanding eventually

## Disclaimer
This script comes as is, feel free to use and modify for any purposes. 
