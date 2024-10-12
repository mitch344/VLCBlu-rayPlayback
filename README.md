# VLC Blu-ray Playback Setup Guide

This guide will help you set up VLC Media Player to play Blu-ray discs on Windows by installing the necessary libraries and configuration files.

## Prerequisites

- Ensure you have VLC Media Player installed on your system.

## Instructions

### Step 1: Download Required DLL Files

1. Visit the Doom9 forum thread: [Doom9 Forum - AACS and BD+ libraries](https://forum.doom9.org/showthread.php?t=176924).
2. Download the following DLL files:
   - `libaacs.dll`
   - `libbdplus.dll`
   - `libgcrypt-20.dll`
   - `libgpg-error6-0.dll`

### Step 2: Place DLL Files

1. Navigate to the VLC installation directory:
C:\Program Files\VideoLAN\VLC

2. Copy the downloaded DLL files into this folder.

### Step 3: Download VM Files

1. In the same Doom9 forum thread, locate and download the VM files (bin files).
2. Create a folder named `vm0` in any preferred location.
3. Place the downloaded VM files into the `vm0` folder.

### Step 4: Download Cached BD+ Tables

1. Download the cached BD+ tables (bin files) from the Doom9 forum.
2. Create another folder named `convtab` in any preferred location.
3. Place the cached BD+ tables into the `convtab` folder.

### Step 5: Copy Folders to %APPDATA%

1. Open the Run dialog by pressing `Win + R`.
2. Type `%APPDATA%` and hit Enter.
3. Copy both the `vm0` and `convtab` folders into the `%APPDATA%` directory.

### Step 6: Download KEYDB.cfg File

1. Download the `KEYDB.cfg` file from the following link: [KEYDB.cfg Download](http://fvonline-db.bplaced.net/).
2. Create a new folder named `aacs` and place the `KEYDB.cfg` file inside it.
3. Copy the `aacs` folder to the `%APPDATA%` directory.

## Conclusion

After completing these steps, you should be able to play Blu-ray discs in VLC Media Player. If you encounter any issues, ensure all files are correctly placed and that your VLC version is up to date. 

**Important:** Make sure to select the "No Blu-ray menu" option in VLC for playback. Alternatively, you can run your discs via the command line:
"C:\Program Files\VideoLAN\VLC\vlc.exe" bluray:///D: --fullscreen --no-bluray-menu
