<div align="center">
<h1>Emina-Cli <sup><sub><sup>(termux) v1.0.0</sup></sub></sup></h1>

Yet Another Simple but Powerful Anime **Streamer/Downloader**


[![Main](https://img.shields.io/badge/Maintainer-TheGlockMisc-green?style=flat)](https://github.com/TheGlockMisc)
[![Main](https://img.shields.io/badge/Maintainer-Zudeath-green?style=flat)](https://github.com/Zudeath)
![Main](https://img.shields.io/badge/OS-Android-blue?style=flat)
![Main](https://img.shields.io/badge/Status-Working-green?style=flat)

[Watch Usage Demo Here](https://youtu.be/YkSA9CnnbzU)
</div>

## Installation
Install Dependencies needed
```
apt update -y
apt install aria2 bc coreutils make ncurses-utils -y
```

Now Install it
```
~# git clone -b emina-termux https://github.com/TheGlockMisc/emina-cli.git
~# cd emina-cli
~# sudo make
```
## Usage
Its Simple..
```
Usage: emina-termux -s "<search query>" -e "[Episode]" -q "High" [--dub]
Usage: emina-termux [arguments...]
```
+ Inputs

| Inputs | Posible Values |
| ------------- | ---------- |
| Episode | All Episodes Possible, Special Episodes (Ex. 6.5) |
| Quality | high, normal, low |

## Prerequisites 
+ *Grep*
+ *MPV* (Available on Playstore)
+ *Aria2c*
+ *Sed*
+ *Awk*
## Option / Args
```
Options:
   -v                          : Show the version of the script
   -s "<search query>"         : Search Anime
   -e "[episode]"              : Number of Episode
   -q "[quality]"              : Quality of Video
   -p "[number]"               : Specify Picks in Anime Selection
   -t "[server]"               : Specify Server (default, 1)
   --dub                       : Switch to Dub Mode
   -d                          : Switch to Download Mode
   -h                          : Show this help

Misc:
   -H                          : Print History File
   -D                          : Clear History File
   -b                          : Play Anime from History
```
<details>
<summary>Additional Infos...</summary>
 
+ Option "-t" will specify which server will used to Stream/Download the file, if this argument presented it will ignore the Config File where the automation stored to set the server..

+ Option "--dub" will change Mode, (Default: None).
    + dub                        : Switch to Dub Mode (Dubbed Anime Only)

+ Option "-q" flag is ignored when downloading Range of Episodes (Default: High)
</details>

## Features
+ You can Change Servers and Other Automations to make your Life Easier
```
~# nano /data/data/com.termux/files/etc/emina/down.conf
```

| Variable | Posible Values |
| ------------- | ---------- |
| Server | default, 1 |
| Video Player | mpv, others |
| Default Quality | high , low |
| Download Mode | 1 |

+ Bulk Downloads
`Ex. [+] Episode: 1-7`
+ Supported Special Episodes
`Ex. [+] Episode: 6.5`

## What's New? (v1.0.0)
```diff
+ Fixed all Servers
+ Stable Release
+ Lightweight
+ Improved Menu
- Shrinks Dependencies
```

## Bugs & Issues
+ If You Found Some Bugs, Feel Free to Create a New Issue (PRs OPEN)
