<div align="center">

---

### 🌯 **Purchase my first commercial game on Steam!**
**[Beso's Shawarma](https://store.steampowered.com/app/4186870/Besos_Shawarma/?beta=0)** — *A short, narrative-driven horror game.*

[![Steam Wishlist](https://img.shields.io/badge/Wishlist%20on-Steam-black?style=for-the-badge&logo=steam&logoColor=white)](https://store.steampowered.com/app/4186870/Besos_Shawarma/?beta=0)

---

</div>

# Hollow Knight for the PS Vita
This repository contains the necessary patches to create fully functional files for running Hollow Knight on the PS Vita.

**IMPORTANT:** You must own **Hollow Knight** on **Steam** or **GOG** to use this patch!  

---
Porting this game to the PS Vita was a significant challenge, requiring compromises and adjustments to accommodate the console’s technical limitations.  
While it’s not perfect and may never be, it’s in reasonably good shape to let you enjoy this amazing game.  

### Compromises  
- **Texture downsizing**: Most textures were reduced in size.  
- **Frame rate**: Capped at 30 FPS but may drop in larger scenes with multiple enemies (until some are defeated).  
- **Audio glitches**: Sounds may occasionally be glitchy.  
- **Loading times**: Scenes take longer to load due to the Vita’s I/O speeds.  

### Known Issues  
- Audio can stutter for a moment when going into or coming out of a loading screen.
- Brief hitches the first time some effects or enemies appear in a session.
- Memory use grows over very long sessions, so an occasional restart will bring the loading times down.

**If you want to support the project, you can leave a tip on one of these websites:**

[Ko-Fi](https://ko-fi.com/patnosd) | [Patreon](https://www.patreon.com/PatnosD) | [PayPal](https://paypal.me/DPatnosD) | [Afdian](https://afdian.com/a/PatnosD)

## PS VITA Set up

In order to have the best possible experience, I recommend using the following plugins (which you can find online):
- `ioplus.skprx` (Required)
- `NoTrpDrm.suprx` (Optional | Used for Trophies)

**+ Full CPU Overclock (500Mhz)**

## Instructions

### Prerequisites
1. Install the Hollow Knight `.VPK` using **VitaShell** or download it straight from **VitaDB** on your PS Vita.  
   *Do not attempt to launch the game yet, as it will crash without the required files.*
2. Ensure you have purchased and downloaded the game from **Steam** or **GOG**.
3. Overclocking is necessary to run the game properly.

---

### Patching Process (Steam & GOG)

1. Visit the **Releases** page of this repository and download the patch zip for your version of the game (`HollowKnightVitaSTEAM.zip` or `HollowKnightVitaGOG.zip`).
2. Extract the downloaded zip to a folder on your PC.
3. Copy your game data into the newly extracted patch folder:
   - **For Steam:** Copy the `Hollow Knight` folder (located in `.../steamapps/common/`).
   - **For GOG:** Copy the `Hollow Knight_Data` folder (located in your GOG installation path).

   *Your folder structure should look like this:*
   ```text
   └── HollowKnightVitaPatch/
    ├── Hollow Knight/          <- (Steam)
    │   -- OR --
    ├── Hollow Knight_Data/     <- (GOG)
    ├── vcdiff/
    ├── APPLYPATCH.bat
    ├── deterministic.exe
    └── xdelta3-x.x.x-x86_64.exe

```

4. Run `APPLYPATCH.bat` and wait for the process to complete (this can take 10-25 minutes depending on your system).
5. Once completed, you will see a new file named `HollowKnightVITA.zip`.
6. Using **VitaShell**, connect your PS Vita to your PC and extract the contents of `HollowKnightVITA.zip` *(around 770MB)* to `ux0:app/HKVT12222/`.
*Your `HKVT12222` folder on your Vita should look like this:*
```text
└── ux0:app/HKVT12222/
 ├── Media/
 ├── sce_module/
 ├── sce_sys/
 ├── archive.psarc
 └── eboot.bin

```


7. When prompted, select **Replace the files in destination**.
8. If you encounter any issues, take a look at the [Troubleshooting](https://www.google.com/search?q=%23troubleshooting) section below.
9. Launch the game and enjoy!

---

### Troubleshooting

* Ensure that your PS Vita is properly overclocked if you run into a poor framerate.
* Verify that you have the correct game version (Steam or GOG) and downloaded the matching patch.
* If `ux0:app` does not appear in File Explorer, make sure you have visibility of hidden directories enabled in Windows.

---

### Disclaimer

This patch requires a legally purchased copy of Hollow Knight.
