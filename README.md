# Hollow Knight for the PS Vita
This repository contains the necessary patches to create fully functional files for running Hollow Knight on the PS Vita.

**IMPORTANT:** You must own **Hollow Knight** on **Steam** or **GOG** to use this patch!  
**NOTICE:** Overclocking is required, and only the **Windows** version of the game is supported.

---

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
    ├── xdelta3
    └── xdelta3-x.x.x-x86_64.exe
```
4. Run `APPLYPATCH.bat` and wait for the process to complete (this can take 15–25 minutes depending on your system).
5. Once completed, you will see a file named `HollowKnightVITA.zip`.
6. Using **VitaShell**, connect your PS Vita to your PC and copy the extracted contents of `HollowKnightVITA.zip` (_around 390–450MB_) to `ux0:app/HKVT12222/`.
   **Note:** Your `HKVT12222` folder on your Vita should look like this:
```
   └── HKVT12222/
    ├── Media/
    └── sce_module/
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
    ├── xdelta3
    └── xdelta3-x.x.x-x86_64.exe
```
4. Run `APPLYPATCH.bat` and wait for the process to complete (this can take 15–25 minutes depending on your system).
5. Once completed, you will see a file named `HollowKnightVITA.zip`.
6. Using **VitaShell**, connect your PS Vita to your PC and copy the extracted contents of `HollowKnightVITA.zip` (_around 300–400MB_) to `ux0:app/HKVT12222/`.
   **Note:** Your `HKVT12222` folder on your Vita should look like this:
```
   └── HKVT12222/
    ├── Media/
    └── sce_module/
```
7. When prompted, select **Replace the files in destination**.
8. if you encounter any issues take a look at the [Troubleshooting](#troubleshooting) section
9. Launch the game and enjoy!

---

### Troubleshooting
- Ensure that your PS Vita is properly overclocked.  
- Verify that you have the correct game version (Steam or GOG) and have followed the steps for your version.
- If `ux0:app` does not appear in File Explorer, make sure you have visibility of hidden directories enabled.

---

### Disclaimer
This patch requires a legally purchased copy of Hollow Knight.
