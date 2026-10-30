# Loading Screen

<details>
<summary>▶️ SHOW</summary>
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/0a0afad5-241f-4079-865d-c33ef0d04d32" />

If you get stuck at this screen, just give it a few minutes and it will eventually load *(note that the window may freeze and say "not responding" aswell but give it 5-10min and it should be fine).*

***(This also applies if for whatever reason you need to reload your resourcepacks)***


* If for some reason refuses to load, or if you're faced with a crash, make sure you have at least 8GB ram allocated: 
  *(input the JVM argument:*
  
     `Xmn10G-Xms8G` *(at the start)*
     and
     `-XX:+UnlockDiagnosticVMOptions -XX:ThreadPriorityPolicy=1 -XX:+UseZGC -XX:+ZGenerational` *(at the end)* 
     
  *in your Minecraft launcher instance profile, watch [this](https://www.youtube.com/watch?v=EeoqVwmvv2U) if you need to learn how).* 
  *also make sure you don't replace your directory path etc*
  
### What the arument does:
* -Xmx10G: Sets the maximum RAM the game can use to 10 Gigabytes.
* -Xms8G: Allocates 8 Gigabytes of RAM instantly at startup to prevent memory crashes. 
* -XX:+UnlockDiagnosticVMOptions: Unlocks Java's hidden expert settings so you can use the advanced tweaks below.
* -XX:ThreadPriorityPolicy=1: Forces Windows to prioritize Minecraft's engine threads, reducing micro-stuttering in-game.
* -XX:+UseZGC -XX:+ZGenerational: Activates Java's newest sub-millisecond memory cleaner, completely eliminating periodic lag spikes in heavy modpacks.

¤¤¤ Disclaimer
* This modpack is right now quite heavy so we recommend **at least 8GB RAM** to run it.
* The `Xmx` and `Xms` arguments are depending on how much RAM your system has *(i.e you can't put 10G if your system only has 8GB ram, and it is **NOT** recommended to allocate the full system RAM - this will most likely cause your system to freeze and/or crash).*

If this doesn't fix the issue, please open a ticket in the [discord](https://discord.gg/CkaUdd5YDk) or submit an issue here on GitHub.
</details>


# Resource pack adding/removing

<details>
<summary>▶️ SHOW</summary>
 
### Step 1

Firstly, you need to navigate to your instance folder.
Assuming you run this on the ***CurseForge Launcher***, you can easily find the folder by clicking the 3 dots to the left of "PLAY".

![Step 1](<RSP tut 1.png>)


### Step 2
Click on "Open Folder"

![Step 2](<RSP tut 2.png>)

This should open the instance folder for you, and within that there should be a file called "**`options.txt`**", open it *(using Notepad, Notepad++, VSCode or any other text editing software)* and move to **Step 3**

![Step 2.5](<RSP tut 2.5.png>)


### Step 3

There is a lot of text here so to make it easier for you, press **`Ctrl`** + **`F`**, this will open a search bar for the .txt file.

![Step 3](<RSP tut 3-1.png>)

Search for "resourcepack", and it will jump to the location for it.


### Step 4

Here, you have to type the names of the resourcepacks you want and place them in the correct loading order.

Here is an example what it would look like if you only want to add **Faithful 64x**

![Just Faithful 64x](<RSP tut 4.png>)

Here is another example with all the packs except Fresh Animations and add-ons:

![All the packs -FA](<RSP tut 4.5.png>)


<details>
<summary>Example</summary>
resourcePacks:["file/5.1.1. - (OPTIONAL) SodiumTranslations.zip","file/4.1.1. - a §bDer's Shaded Font §864x §3v21§8.zip","file/Required/3.1.4. - Icon Xaero's 1.22.zip","file/Recommended/3.1.1. - Excalibur - Xaero's World Map.zip","file/3.1.2. - Xaero's Modded Support 1.21.zip","file/2.1.8 - Jade Better DARK.zip","file/2.1.7. - Better_withered_hearts.zip","file/2.1.5. - Recolourful Containers DARK 3.1.3 (1.19.4+).zip","file/2.1.4. - Unique Dark Expansion pack.zip","file/2.1.2. - Unique Dark - Mekanism 1.20.2-1.21 v2.1.zip","file/2.1.1. - Unique Dark Refined - Lite - 1.20.2-26.x.zip","file/Recommended/1.2.24 - Waystones Emissive.zip","file/Recommended/1.2.23 - Waystones PBR.zip","file/Recommended/1.2.18 - Creepers Reforged v1.1.2.zip","file/Recommended/1.2.17 - §9Azu's Enhanced Zombie Variants v1.2.zip","file/Recommended/1.2.15 - §6Drodi's Villagers [V2.8].zip","file/Recommended/1.2.12 - AL's Spiders Revamped 1.3.zip","file/1.2.20. - Freshly Modded 3.0.5.zip","file/Required/1.3.28 - §e{Vanilla}EatingAnimationsMoreCompat.zip","file/Required/1.3.27. - §eEatingAnimationsMoreCompat1.20-26.x.zip","file/Required/1.3.26. - EatAnimation Farmer's Delight's Compat 1.20-26.x.zip","file/Recommended/1.1.1. - Visual Effects+.zip","file/Recommended/0.2.27 - Mystical 3DRetextured+.zip","file/Recommended/0.2.26 - Fyoncle's 3D Trims.zip","file/0.2.24. - Punched Better, Fresher 3D books.zip","file/0.2.23. - Animated Items 1.21.x-26.3 - v1.6.3.zip","file/0.2.18. - Enchanting Table Magic Circle v.2.5 (1.20.5 - 1.21.8).zip","file/Recommended/0.2.22 - Fresh Ores and Ingots.zip","file/Recommended/0.2.21 - rainbows-foliage-polytone-edition-v2.1.zip","file/Recommended/0.2.20 - Drigo 3D Lantern`s x Punchy.zip","file/Recommended/0.2.19. - Enchantment Outlines.zip","file/0.2.17.5 - SeamlessAO-Glow.zip","file/0.2.17 - SeamlessAO-Border.zip","file/Optional/0.2.15. - §3Fresh §bFlower Pots.zip","file/Optional/0.2.14. - §3Fresh §bFlower Pots Compats§r.zip","file/Optional/0.2.13. - §3Fresh §bFlower Pots Rotated.zip","file/0.2.11 - CraftGlow Round Barrel.zip","file/0.1.9. - Fluffy Carpets v1.1.zip","file/0.1.8. - Fancy Crops v1.3.zip","file/0.1.6 - Round_Cacti v3.zip","file/0.1.5. - Round-Trees-8.4.zip","file/Recommended/0.1.7 - Better Beds.zip","file/Recommended/0.1.4. - §f§lActually §6§l3D §fBlocks & Items!§7.zip","file/0.1.3. - FFC Clean Glass 64x v1.0.1.zip","file/0.1.2. - Faithful 64x - AppleSkin.zip","file/0.1.1. - Faithful 64x - Release 6.zip","vanilla","program_art","fabric","mod_resources","berezka","moonlight","eatinganimations","quest_enhance","epicfight","colourful_slimes","neovitae","tacz","compatlink","boatiview"]

</details>   
   
You can if you want, just copy the text above in the "example" after you've downloaded them and put it there, packs that you don't have installed won't be loaded and after a restart remove the strings that are not available.

### Step 5

Press `Ctrl` + `S` to save the changes or in the top left "`File`" > "`Save`" and close the window.

Now you're all done!
Just boot up your instance and enjoy!

</details>

<!-- GitHub native alerts cannot render inside collapsible sections. Callouts use Shields.io badges plus Markdown tables. -->
# Failed to install **v0.2.0 Pre-Release #2**

![Minecraft](https://img.shields.io/badge/Minecraft-1.21.1-4c9f38?style=flat-square) ![Loader](https://img.shields.io/badge/Loader-NeoForge%2021.1.262-f97316?style=flat-square) ![Status](https://img.shields.io/badge/Status-Alpha%20Pre--release-b96ad9?style=flat-square)

<details>
<summary><strong>▶️ SHOW</strong></summary>


# 🛠️ The Last Circuit Pre-Release #2 — Installation Guide

> **Applies to:** The Last Circuit **v0.2.0-Alpha (Pre-release #2)**  
> **Minecraft:** Java Edition 1.21.1  
> **Mod loader:** NeoForge 21.1.262  
> **Recommended allocated RAM:** 8–12 GB  
> **Status:** Alpha / pre-release — installation and compatibility issues may still occur.

Welcome to **The Last Circuit**! This guide covers installation through the CurseForge app and the **manual mods** needed to complete the setup.

<details>
<summary><strong>📥 1. Install through CurseForge</strong></summary>

1. Install and open the [CurseForge app](https://www.curseforge.com/download/app).
2. Select **Minecraft: Java Edition**.
3. Open **Browse** and search for **The Last Circuit** by **ImFloof**.
4. Select the modpack and install **v0.2.0 Pre-release #2**.
5. Allow CurseForge to finish downloading and installing the profile **before launching Minecraft**.

**Modpack page:** [The Last Circuit on CurseForge](https://www.curseforge.com/minecraft/modpacks/the-last-circuit)

| ![IMPORTANT — Before you launch](https://img.shields.io/badge/IMPORTANT-BEFORE%20LAUNCH-d29922?style=for-the-badge) |
|:--|
| **Do not launch the modpack yet.** Some mods must be added manually before the first launch. |

</details>

<details>
<summary><strong>📂 2. Find your mods folder</strong></summary>

1. In CurseForge, go to **My Modpacks**.
2. Find and open your installed **The Last Circuit** profile.
3. Use the profile menu (usually **three dots**) and choose **Open Folder**.
4. Open the **`mods`** folder inside that profile.

The default Windows location is similar to:

```text
C:\Users\<your-username>\curseforge\minecraft\Instances\<your-profile-name>\mods\
```

Your actual location may differ if you changed the CurseForge installation directory.

</details>

<details>
<summary><strong>🧩 3. Install The Broken Script — REQUIRED</strong></summary>

**The Broken Script (TBS) is required for the intended experience.** It is distributed through **Modrinth**, not CurseForge.

1. Open the [official The Broken Script page on Modrinth](https://modrinth.com/mod/the-broken-script).
2. Download the **Minecraft 1.21.1 / NeoForge** version specified for this pre-release. The currently documented pack version is [The Broken Script 2.0.5](https://modrinth.com/mod/the-broken-script/version/aD9cfKVd).
3. Move the downloaded **`.jar`** file into the profile's **`mods`** folder.
4. Do **not** extract the `.jar` file.

| ![WARNING — Official downloads only](https://img.shields.io/badge/WARNING-OFFICIAL%20SOURCE%20ONLY-e3b341?style=for-the-badge) |
|:--|
| Download TBS **only from its official Modrinth page**. The developer states that copies uploaded elsewhere are unauthorized and may be unsafe. |

</details>

<details>
<summary><strong>👁️ 4. Check void.jar — REQUIRED FOR FULL EXPERIENCE</strong></summary>

**void.jar** is paired with The Broken Script. Its CurseForge dependency metadata previously caused the installer to attempt downloading an unavailable CurseForge copy of TBS (`project-1240986`).

For **Pre-release #2**, void.jar has been marked as an **optional CurseForge dependency** as a possible workaround. **This workaround is not yet confirmed to resolve installation errors.**

1. Check whether a file named similarly to **`thevoid-1.11.0-neoforge-1.21.1.jar`** is already present in your `mods` folder.
2. **If it is present:** Leave it there. **Do not add a duplicate.**
3. **If it is missing:** Download **void.jar 1.11.0 for Minecraft 1.21.1 / NeoForge** from its [official CurseForge file page](https://www.curseforge.com/minecraft/mc-mods/void-jar/files/8520286) and place the `.jar` file in `mods`.
4. Make sure **both TBS and void.jar** are present before starting Minecraft.

| ![NOTE — Dependency information](https://img.shields.io/badge/NOTE-DEPENDENCY%20INFORMATION-0969da?style=for-the-badge) |
|:--|
| Marking void.jar as an optional dependency does **not** make The Broken Script optional for gameplay. The void.jar author warns that some events will break without TBS. |

### Your folder should now contain at least

```text
<The Last Circuit profile>/
└── mods/
    ├── ... (mods installed by CurseForge)
    ├── <the-broken-script-file>.jar
    └── thevoid-1.11.0-neoforge-1.21.1.jar
```

**Only one copy of each mod should be installed.** The TBS filename is an example placeholder; keep the actual filename of the official download.

</details>

<details>
<summary><strong>📦 5. Other manual downloads</strong></summary>

The pre-release changelog also lists the following additions. Read their individual project pages and check version compatibility before installing them:

| Mod / component | Status | Official source |
|---|---|---|
| **AE2 Dynamic Trees Fix** | Required compatibility fix | [Modrinth](https://modrinth.com/mod/ae2-dynamic-trees-fix) |
| **The Broken Script: BLACKOUT** | Manual addon listed for this pre-release | [Modrinth](https://modrinth.com/mod/tbs_blackout) |
| **FixSodiumShaderLoader** | Recommended if you use shaders with Voxy LoD | [GitHub](https://github.com/coco875/Fix-sodium-ShaderLoader) |
| **Essential Mod** | Optional; not part of the core manifest | [Modrinth](https://modrinth.com/mod/essential) |

**Voxy:** The pre-release uses an unofficial NeoForge 1.21.1 backport which cannot be redistributed with this modpack. If you want Voxy, follow the instructions in the [pre-release changelog](https://github.com/ImFloofo7/thelastcircuit/tree/Latest/All%20Changelogs) and use the [unofficial backport source repository](https://github.com/NHblock-Johnsnow/neo-voxy-multiversion). It must be built separately; do not download JARs from untrusted mirrors.

**Resource packs:** Some packs require separate downloads due to licensing restrictions. See the [resource pack list and order](https://docs.google.com/spreadsheets/d/1aFkWyf8V0sgwXtd2bKsqFTWQClMtUoas1fNS3lf8A84/edit?usp=sharing) and the [troubleshooting and installation guide](https://github.com/ImFloofo7/thelastcircuit/blob/Latest/Troubleshooting/troubleshooting%20and%20knows%20issues.md#resource-pack-addingremoving).

| ![CAUTION — Back up important worlds](https://img.shields.io/badge/CAUTION-BACK%20UP%20YOUR%20WORLDS-cf222e?style=for-the-badge) |
|:--|
| Some horror mods include intentionally disruptive mechanics, including loud sounds, flashing visuals, pop-ups, forced disconnects and possible world deletion. **Back up important worlds** and review the relevant mod settings before playing. The Broken Script: BLACKOUT in particular documents world-deletion and ban mechanics that should be checked in its configuration. |

</details>

<details>
<summary><strong>🚀 6. Launch The Last Circuit</strong></summary>

1. Return to CurseForge and open **My Modpacks**.
2. Select **The Last Circuit** and click **Play**.
3. Allow Minecraft to finish starting; the first launch may take considerably longer than usual.
4. Before creating an important survival world, test that **Singleplayer** opens and a **new test world** can be created successfully.

| ![NOTE — First world creation](https://img.shields.io/badge/NOTE-WORLD%20CREATION-0969da?style=for-the-badge) |
|:--|
| During **“Preparing for world creation...”**, Windows may temporarily show **“Not Responding”** while Minecraft processes large numbers of datapacks, recipes and resources. This **does not automatically mean the game has crashed**. Avoid force-closing it solely because of a temporary freeze. |

For alpha testing, consider using the `/safemode` command recommended in the pre-release notes for The Broken Script, where applicable, to reduce the risk of intrusive lock mechanics during debugging.

</details>

<details>
<summary><strong>🛠️ 7. Troubleshooting</strong></summary>

### CurseForge says “Operation failed” or “An unexpected error occurred”

If installation fails with an error like:

```text
Unable to install the following addon dependency:
'project-1240986' - 1240986
```

CurseForge is still attempting to retrieve **The Broken Script's old CurseForge project** through dependency resolution.

**Important:** Manually installing TBS **afterward will not fix a CurseForge installation that never completes**. The optional-dependency change in Pre-release #2 is a test, not a confirmed fix.

- Retry once to rule out a temporary issue.
- Check that you selected **Pre-release #2**, not an older release.
- If the same `1240986` error persists, report it to the project. A new export without the offending `void.jar` manifest entry may be needed; users cannot reliably solve this by editing their local `mods` folder before the installer finishes.

### Minecraft fails to start after adding the manual mods

- Verify that every manual download supports **Minecraft 1.21.1 and NeoForge**.
- Check for **duplicate versions** of TBS or void.jar.
- Ensure the files are `.jar` files **directly inside** the profile's `mods` folder, not inside another folder or ZIP.
- Check the version-specific changelog for known conflicts and required manual fixes.
- Attach `latest.log` and, if one was generated, the matching `crash-reports/*.txt` file when reporting the issue.

### World creation appears frozen

This is a known issue in the alpha build. Wait for the game to finish processing before assuming it crashed. If it eventually exits or repeatedly fails, provide the logs rather than relying only on the Windows “Not Responding” message.

</details>

<details>
<summary><strong>💬 8. Support and bug reports</strong></summary>

If you encounter installation errors, crashes or missing mods, please include:

- Your **The Last Circuit version** (for example, Pre-release #2).
- Whether installation through CurseForge **completed successfully**.
- The **exact error message** and the steps leading up to it.
- `latest.log`, relevant crash reports or a CurseForge/Overwolf logs ZIP, where applicable.

**Support channels:**

- [Official Discord](https://discord.gg/A3TFF6TqEU)
- [GitHub Issues](https://github.com/ImFloofo7/thelastcircuit/issues)
- [The Last Circuit on CurseForge](https://www.curseforge.com/minecraft/modpacks/the-last-circuit)

</details>

---

*Thank you for playing and supporting The Last Circuit! 💙💜*

</details>
