# Pokémon FireRed Ironmon Kaizo — French Patch 1.3

> 🇫🇷 [Lire ce README en français](README.md)

French adaptation of **Faster FireRed** for a **French vanilla Pokémon FireRed ROM**, primarily intended for **IronMON / Ironmon Kaizo** runs.

This repository / release only provides a **patch**. No Pokémon ROM is distributed.

---

## Table of Contents

1. [Patch origin](#1-patch-origin)
2. [Changes included](#2-changes-included)
3. [Applying the patch to a French vanilla ROM](#3-applying-the-patch-to-a-french-vanilla-rom)
4. [Fully translated French Ironmon Tracker](#4-fully-translated-french-ironmon-tracker)
6. [External links and credits](#6-external-links-and-credits)

---

## 1. Patch origin

This project is based on the US **Faster FireRed** patch created by **DrMaple**:

- **Faster FireRed**: https://github.com/DrMaple/Faster-FireRed

The original project is a patch for **Pokémon FireRed (Rev 1 / 1.1)** that adds several quality-of-life improvements designed specifically for IronMON runs.

This French version uses that work as its base and adapts it to a **French vanilla Pokémon FireRed ROM**.

The chosen base is the **No Hidden Item Marks** variant, preserving hidden items as genuinely hidden items.

### Reference French ROM

The current patch was developed and tested using the French reference ROM used throughout development.

- **Format**: GBA
- **Reference French ROM SHA-1**: `FC663907256F06A3A09E2D6B967BC9AF4919F111`

Before applying the patch, it is strongly recommended to verify that your dump matches this ROM.

---

## 2. Changes included

### Changes inherited from Faster FireRed

The patch keeps the main quality-of-life improvements from the original Faster FireRed project, including:

- faster start to the adventure;
- shortened Oak's Parcel quest;
- automatic prompt to use another Repel when the current one expires;
- Pokémon Name Raters added to Pokémon Centers;
- heavily shortened Pokémon Center healing animation;
- selected step items in the Underground Passes and Sevii Islands guaranteed to spawn;
- the item normally obtained from the PC moved to Professor Oak's lab;
- Bill no longer automatically asks you to travel to the Sevii Islands after Blaine; he remains available in the Cinnabar Island Pokémon Center so the trip can still be started manually;
- additional quality-of-life NPC adjustments designed for IronMON runs;
- a Nurse added to Viridian Forest according to Faster FireRed's original rules;
- **no visual markers for hidden items** in this build.

For the full list of upstream changes, see DrMaple's repository:
https://github.com/DrMaple/Faster-FireRed

### French-specific adaptations and changes

This version additionally includes:

- adaptation of Faster FireRed to a **French Pokémon FireRed ROM**;
- French localization / adaptation of patch-specific text and dialogue;
- validated relocation of the PC item to Professor Oak's lab on the French ROM;
- further shortening of the **New Game** introduction by removing intermediate intro screens, allowing the player to reach the actual game setup faster;
- shortened **Bill cutscene in his house on Route 25**;
- shortened dialogue for the **Pokémon Fan Club Chairman in Vermilion City**;
- custom title screen featuring:
  - **ROUGE FEU / IRONMON / KAIZO**;
  - **Patch FR 1.3 made by TensaZangetsu22**;
- graphical adjustments designed to keep the title screen visually consistent with the original Pokémon FireRed presentation.

The overall goal is to preserve the gameplay and intent of the original US patch while providing an experience fully adapted to the French version of the game.

---

## 3. Applying the patch to a French vanilla ROM

### Requirements

You need:

1. your own **French vanilla Pokémon FireRed ROM**;
2. the `.ips` file included with this release;
3. an IPS-compatible patching tool.

**Always keep an untouched backup of your original ROM.**

Do not apply the patch on top of a ROM that is already modified, randomized, or patched.

### ROM verification

The reference French ROM used for this project has the following SHA-1:

- `FC663907256F06A3A09E2D6B967BC9AF4919F111`

If your patching tool displays the ROM SHA-1, verify that it matches before applying the patch.

---

### macOS — recommended method with MultiPatch

On macOS, you can use **MultiPatch**, a native application developed by Sappharad:

https://projects.sappharad.com/multipatch/

MultiPatch supports several patch formats, including **IPS, BPS, UPS, PPF, XDelta, BSDiff and RUP**.

> **Important: MultiPatch is a macOS application.**  
> There are no official MultiPatch builds for Windows or Linux.

#### Installation

1. Download MultiPatch from the official website:
   - https://projects.sappharad.com/multipatch/
2. Open the application.
3. If macOS blocks it from launching, right-click the application and choose **Open**, or allow it from **System Settings > Privacy & Security**.

#### Applying the patch

1. Launch **MultiPatch**.
2. Under **Location of patch file**, select the French patch `.ips` file.
3. Under **Location of file to patch**, select your French vanilla `.gba` ROM.
4. Under **Save patched file as**, choose a new filename, for example:
   - `Pokemon_FireRed_Ironmon_Kaizo_FR.gba`
5. Click **Apply Patch**.
6. Wait for MultiPatch to confirm that the patch was applied.
7. Load the newly created ROM in your emulator.

Do not overwrite your original ROM; always keep a clean backup.

---

### Windows — Rom Patcher JS

MultiPatch is not officially available for Windows.

The easiest option is **Rom Patcher JS**:

https://www.marcrobledo.com/RomPatcher.js/

1. Open Rom Patcher JS in your browser.
2. Under **ROM file**, select your French vanilla ROM.
3. If possible, verify that its SHA-1 matches:
   - `FC663907256F06A3A09E2D6B967BC9AF4919F111`
4. Under **Patch file**, select the French patch `.ips` file.
5. Click **Apply patch**.
6. Save the generated ROM under a new filename.
7. Load that ROM in your emulator.

You may also use any compatible local Windows IPS patcher if you prefer an offline tool.

---

### Linux — Rom Patcher JS

MultiPatch is not officially available for Linux.

The easiest method is **Rom Patcher JS**:

https://www.marcrobledo.com/RomPatcher.js/

1. Open Rom Patcher JS in your browser.
2. Load your French vanilla `.gba` ROM.
3. Load the `.ips` patch.
4. Verify the ROM SHA-1 if the tool displays it.
5. Click **Apply patch**.
6. Save the generated ROM under a new filename.

You may alternatively use a native Linux IPS patcher, provided it applies a standard IPS patch without otherwise modifying the ROM.

---

### Universal alternative — Rom Patcher JS

Rom Patcher JS works on **Windows, macOS and Linux** directly from a modern web browser:

https://www.marcrobledo.com/RomPatcher.js/

It is therefore a convenient fallback if you do not want to install a dedicated application.

### Checking the result

After launching the patched game, you should see:

- the custom **Rouge Feu Ironmon Kaizo** title screen;
- the **Patch FR 1.3 made by TensaZangetsu22** credit;
- French text;
- Faster FireRed quality-of-life changes adapted to the French ROM.

If the title screen is corrupted or the game does not boot, first verify that you used the **correct French vanilla ROM** rather than an already-modified ROM.

---

## 4. Fully translated French Ironmon Tracker

A complete French translation of the **Gen 3 Ironmon Tracker** is available in the following fork:

- **French Tracker — `feature/french-complete-translation` branch**  
  https://github.com/TensaZangetsu22/Ironmon-Tracker/tree/feature/french-complete-translation

This project is a fork of the existing Gen 3 tracker maintained here:

- **Original Ironmon-Tracker — besteon**  
  https://github.com/besteon/Ironmon-Tracker

The French translation is currently **complete and awaiting validation** before potential inclusion in a future official Tracker release.

### Using the patched ROM with the Tracker in BizHawk

The Gen 3 Tracker uses Lua scripts. The project requires **BizHawk 2.8 or newer**; on Linux, a newer version is recommended.

1. Download the French Tracker branch.
2. Extract the Tracker folder to a simple location.
   - Avoid cloud-synced folders when possible.
   - Avoid paths containing special characters if you run into file access issues.
3. Start **BizHawk / EmuHawk**.
4. Load your **patched French FireRed Ironmon Kaizo ROM**.
5. In BizHawk, open:
   - `Tools -> Lua Console`
6. In the Lua Console:
   - `Script -> Open Script...`
7. Select:
   - `Ironmon-Tracker.lua`
8. The Tracker should appear and detect the loaded ROM.
9. Configure the Tracker using its Gear icon according to your IronMON preferences.

### Windows

BizHawk is directly supported. Make sure to install the BizHawk prerequisites if required.

### Linux

Prefer the **native Linux build of BizHawk** instead of running the Windows build through Wine / Proton. The Tracker project recommends BizHawk 2.9 or newer on Linux for improved compatibility.

### macOS

BizHawk is not the recommended native option on macOS. If you run BizHawk through **Parallels Desktop**, keeping the Tracker folder inside the Windows VM filesystem rather than a shared macOS folder may help avoid permission issues.

The Tracker can also run with **mGBA**, although Lua display capabilities are more limited than with BizHawk.

Official Tracker installation guide:
https://github.com/besteon/Ironmon-Tracker/wiki/Installation-Guide

---

## 6. External links and credits

### Patch and tools

- **Faster FireRed — DrMaple**  
  https://github.com/DrMaple/Faster-FireRed

- **MultiPatch — Sappharad (macOS)**  
  https://projects.sappharad.com/multipatch/

- **Rom Patcher JS — Marc Robledo**  
  https://www.marcrobledo.com/RomPatcher.js/

### Tracker

- **French Ironmon Tracker fork — TensaZangetsu22**  
  https://github.com/TensaZangetsu22/Ironmon-Tracker/tree/feature/french-complete-translation

- **Original Gen 3 Ironmon Tracker — besteon**  
  https://github.com/besteon/Ironmon-Tracker

- **Tracker Installation Guide**  
  https://github.com/besteon/Ironmon-Tracker/wiki/Installation-Guide

### README

- 🇫🇷 [README français](README.md)

---

## Credits

- **DrMaple** — creator of the original Faster FireRed patch.
- **besteon and Ironmon-Tracker contributors** — development and maintenance of the Gen 3 Tracker.
- **TensaZangetsu22** — French patch adaptation, French-specific modifications, custom title screen, and French Tracker translation.

Pokémon is a trademark of Nintendo / Creatures Inc. / GAME FREAK inc.  
This is an unofficial community project and is not affiliated with Nintendo, Creatures Inc., or GAME FREAK.
