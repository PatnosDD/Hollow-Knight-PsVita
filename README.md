# Hollow Knight for the PS Vita
This repository contains the necessary patches to create fully functional files for running Hollow Knight on the PS Vita.

**IMPORTANT:** You must own **Hollow Knight** on **Steam** or **GOG** to use this patch!  

---
Porting this game to the PS Vita was a significant challenge, requiring compromises and adjustments to accommodate the console’s technical limitations.  
While it’s not perfect and may never be, it’s in reasonably good shape to let you enjoy this amazing game.  

Disclaimer for new players. The tutorial scene is the only scene with that kind of horrific performance, After that scene, experience is better.

### Compromises  

- **Texture downsizing**: Most textures were reduced in size.  
- **Frame rate**: Capped at 30 FPS but may drop in larger scenes with multiple enemies (until some are defeated).  
- **Audio glitches**: Sounds may occasionally be glitchy.  
- **Loading times**: Scenes take longer to load due to the Vita’s I/O speeds.  

### Known Issues  

- **Lower FPS in busy areas**: Performance drops in some scenes with many enemies (**the tutorial scene has the most noticeable lag**).  
- **Longer load times for larger scenes**: Bigger areas may take extra time to load.  
- **Periodic lag spikes**: Once every minute or so, you may encounter a lag spike caused by various factors.  

**If you want to support the project, you can leave a tip on one of those websites:**

Ko-Fi: https://ko-fi.com/patnosd

Patreon: https://www.patreon.com/PatnosD

PayPal: https://paypal.me/PatnosDD

Afdian: https://afdian.com/a/PatnosD

## PS VITA Set up

In order to have the best possible experience, I recommend you to use following plugins (that you should be able to find somewhere on the net) :
- ioplus.skprx (Required)
- iostaging.skprx (Optional)

**+ Full CPU Overclock (500Mhz)**


## Instructions

### Prerequisites
1. Install the Hollow Knight `.VPK` using **VitaShell** or download it straight from **VitaDB** on your PS Vita.  
   *Do not attempt to launch the game yet, as it will crash without the required files.*
2. Ensure you have purchased and downloaded the game from **Steam** or **GOG**.
3. Overclocking is necessary to run the game properly.

---

### STEAM VERSION
1. Visit the **Releases** page of this repository and download `HollowKnightVitaSTEAM.zip`.
2. Extract the downloaded zip to a folder on your PC.
3. Copy the Steam game folder into the extracted folder.  
   **Note:** Your `HollowKnightVitaPatchSteam` folder should look like this:
```
   └── HollowKnightVitaPatchSteam/
    ├── Hollow Knight/  <- ../steamapps/common/Hollow Knight
    ├── vcdiff/
    ├── APPLYPATCH.bat
    ├── deterministic.exe
    └── xdelta3-x.x.x-x86_64.exe
```
4. Run `APPLYPATCH.bat` and wait for the process to complete (this can take 15–25 minutes depending on your system).
5. Once completed, you will see a file named `HollowKnightVITA.zip`.
6. Using **VitaShell**, connect your PS Vita to your PC and copy the extracted contents of `HollowKnightVITA.zip` (_zip file should be around 380–450MB_) to `ux0:app/HKVT12222/`.
   **Note:** Your `HKVT12222` folder on your Vita should look like this:
```
   └── HKVT12222/
    ├── Media/
    ├── sce_module/
    ├── sce_sys/
    └── eboot.bin
```
7. When prompted, select **Replace the files in destination**.
8. if you encounter any issues take a look at the [Troubleshooting](#troubleshooting) section
9. Launch the game and enjoy!

---

### GOG VERSION
1. Visit the **Releases** page of this repository and download `HollowKnightVitaGOG.zip`.
2. Extract the downloaded zip to a folder on your PC.
3. Copy the GOG game folder into the extracted folder.  

   **Note:** Your `HollowKnightVitaPatchGOG` folder should look like this:
```
   └── HollowKnightVitaPatchSteam/
    ├── Hollow Knight_Data/  <- ../GOG/Hollow Knight/Hollow Knight_Data
    ├── vcdiff/
    ├── APPLYPATCH.bat
    ├── deterministic.exe
    └── xdelta3-x.x.x-x86_64.exe
```
4. Run `APPLYPATCH.bat` and wait for the process to complete (this can take 15–25 minutes depending on your system).
5. Once completed, you will see a file named `HollowKnightVITA.zip`.
6. Using **VitaShell**, connect your PS Vita to your PC and copy the extracted contents of `HollowKnightVITA.zip` (_zip file should be around 380–450MB_) to `ux0:app/HKVT12222/`.
   **Note:** Your `HKVT12222` folder on your Vita should look like this:
```
   └── HKVT12222/
    ├── Media/
    ├── sce_module/
    ├── sce_sys/
    └── eboot.bin
```
7. When prompted, select **Replace the files in destination**.
8. if you encounter any issues take a look at the [Troubleshooting](#troubleshooting) section
9. Launch the game and enjoy!

---

### Transferring Save Files
If you are updating from an older version of the game, your save files need to be moved to a new directory. Follow these steps:

1. **Locate Old Save Files**:  
   Navigate to `ux0:data` and identify all files starting with `user...`.

2. **Move Files**:  
   Copy these files and transfer them to the new save directory:  
   `ux0:data/HollowKnight`.

3. **Verify**:  
   Ensure all save files are properly placed in the `HollowKnight` folder.

---

### Troubleshooting
- Ensure that your PS Vita is properly overclocked.  
- Verify that you have the correct game version (Steam or GOG) and have followed the steps for your version.
- If `ux0:app` does not appear in File Explorer, make sure you have visibility of hidden directories enabled.

---

### Disclaimer
This patch requires a legally purchased copy of Hollow Knight.
