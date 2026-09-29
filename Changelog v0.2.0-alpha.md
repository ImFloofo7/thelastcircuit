# **WORK IN PROGRESS**

<img width="2172" height="724" alt="TCL Banner Alt compressed" src="https://github.com/user-attachments/assets/d0b1f9dc-5e09-4c53-bc24-1944512ae51c" />


# V0.2.0-Alpha IS HERE, **AND IT'S HUGE!**

# 🛠️ Changelog: v0.2.0-alpha

## Mod permissions!


### [Epic Fight "Nightfall"](https://curseforge.com) & [GabouLibs](https://curseforge.com) now included!

Finally managed to come to an agreement on permission of usage for the mods, so they are now included in the modpack!

**HUGE** Thanks to [Gaboouu](https://github.com) & "[Super_awespme_baby](https://curseforge.com)" again for granting me permission to include these in the modpack! ❤️


### Platform changes!
In the requirements of getting permission for said mods were to publish on CurseForge. Together with some technical reasons amongst other, we've decided to switch to CurseForge permanently!
*(Project on Modrinth has been deleted and **`v0.1.0-alpha-r.dev`** is no longer available for the public).*

### New Additions!

[Voxy](https://github.com/NHblock-Johnsnow/neo-voxy-multiversion) - *New LoD rendering mod*
We decided to switch over to Voxy for many reasons, main being that it has better compatibility with various mods and fits our vision better.


***Please note: we do not condone in republishing this modpack without the permission from the author of this modpack anymore.***
*(Please see updated [license](https://github.com))*

---

## ⚙️ Optimizations & Fixes
* **Cleaned Up Codes:** Fixed multiple fatal JSON metadata boot errors *(like "`No key pack_format`")* hidden inside the resource packs.   
* **Launch Performance:** Fixed early launch loading stalls and graphics adapter workarounds by purging legacy translation caches.   
* **Engine Optimizations:** Enhanced thread prioritization and sub-millisecond memory cleanups *("`ZGC`")* to completely eliminate cyclic lag spikes in heavy factory zones.   
* **Optimized overall performance:** We've optimized the game to run smoother thanks to removing modds, adding more compatibility and performance mods.   

***We're constantly working on making the modpack run smoother on all systems, though it is hard for lower-end systems because of the size of this modpack.***


---

## 🎨 Resource Pack Architecture

To make things as seamless as possible for alpha testing, a massive overhaul has been done to the Resource Pack system. All custom assets, dark UI themes, and Fresh Animations patches are now **fully numbered and categorized in their strict logical loading order**.

If the game layout resets or doesn't load them automatically on your first boot, simply move them into the active (`Selected`) column and stack them following their prefix indices:

1. **🧱 Base Overhauls & Block Models (`0.1.1` > `0.1.9`):** Forms the core foundation of your world. This initiates the main Faithful 64x overhaul, custom 3D crops, connected flower pots, seamless ore glows, and base block textures.   
2. **🧬 Fresh Animations Core & Extensions (`1.2.10` > `1.2.19`):** Loads the fundamental resource frameworks first, followed directly by the core Fresh Animations engine, official extensions (`FA+`), and custom entity additions (like Drodi's Villagers).   
3. **⚔️ Combat, Item & Creature Compatibility (`1.3.20` > `1.3.27`):** Integrates specialized creature compatibility patches (`x FA`) cleanly over the core models.   Player combat modifications, weapon shapes, and item action dependencies (like Eating Animations) load right alongside them to prevent visual clipping.   
4. **⚙️ Mod Gränssnitt & Dark Expansions (`2.1.1` > `2.1.9`):** Loads the specialized dark theme configurations for major technology and automation mods (Create, Mekanism, Refined Storage etc).   
5. **🗺️ Maps, Icons & Minimap Fixes (`3.1.1` > `3.1.4`):** Integrates customized map stylings, Excalibur alignment profiles, and icon patches cleanly over the engine layer.   
6. **👑 UI, Fonts, and Core Fixes (`5.1.8` > `6.1.1` - Absolute Top):** Highest loading priority. Activates the custom container shadings, font overhauls (Der's Shaded Font), and global Sodium translation patches over all active asset arrays.   

### Starting with "0.1.1" being at the bottom. - 
*adding 0.1.1 first, 0.1.2 second, etc.*

**Disclaimer!**
Some resourcepacks are built-in with some mods and should be left at the bottom of the loading order, except for "punchy" which should be placed between `1.3.27` and `2.1.1`

---

## 🖥️ MOD updates, removals and added.


## ▶️ **Added:**

## **New Features & Content**
*The following mods are new additions to the modpack that make changes to one thing or another.*    
     *   **[Laser IO](https://www.curseforge.com/minecraft/mc-mods/laserio)** - *EnderIO Pipes but reworked and additional content*   
     *   **[TacZ: AoS](https://www.curseforge.com/minecraft/mc-mods/tacz-art-of-sniping)** - *TACZ: AoS lets you snipe entities from extreme distances with realistic ballistics.*   
     *   **[Epic Fight - Bosses'Rise](https://www.curseforge.com/minecraft/mc-mods/bossesrise)** - *Adds souls-like bosses, dungeons and loot.*   
     *   **BetterEnd Cities** - *Generates unique city structures and progression markers throughout the End dimension.*   
     *   **Bio-Scanner** - *Faction tracking and specialized entity identification.*   
     *   **[TacZ Attributes](https://www.curseforge.com/minecraft/mc-mods/tacz-attributes)** - *Adds more than 250 attributes to TacZ weapons*   
     *   **[LittleTiles](https://www.curseforge.com/minecraft/mc-mods/littletiles)** - *Adds micro (pixel) blocks*   
     *   **[Advanced Hook Launchers](https://www.curseforge.com/minecraft/mc-mods/advanced-hook-launchers)** - **   
     *   **Diamond Vein** - *Mining optimizations and automated scanning adjustments.*   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **[Distant Friends](https://www.curseforge.com/minecraft/mc-mods/distant-friends)** - *Adds stalking player-like mobs that creep at you from a distance.*   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   
     *   **** - **   

     
## **QoL**
*Small mods that doesn't really add any "new content", but are still nice to have.*    
    *   **BetterF3 Spark Module** - *Addon for Directly links hardware monitoring with the F3 menu interface.*       
    *   **[Quick Pack](https://www.curseforge.com/minecraft/mc-mods/quick-pack)** - *Improves datapack & resourcepack zip gile loading times.*   
    *   **[Punchy!](https://www.curseforge.com/minecraft/mc-mods/punchy)** - *Engine for various first-person animations.*   
    *   **[Thunderhead](https://www.curseforge.com/minecraft/mc-mods/thunderhead)** - *Lightning & Thunder overhaul.*   
    *   **[SeeU](https://www.curseforge.com/minecraft/mc-mods/seeu)** - *Makes distant players visible far beyond canilla entity tracking, Compatible with Voxy*   
    *   **[Voxy](https://github.com/NHblock-Johnsnow/neo-voxy-multiversion)** - *A LoD renderer*   
    *   **[Roxy](https://www.curseforge.com/minecraft/mc-mods/roxy)** - *Allows Voxy (that is for fabric) to work on NeoForge*   
    *   **AAA World** - **   
    *   **FancyMods BetterEnd Tweaks** - *Balance adjustments and biome-specific block variants.*   
    *   **Search for Iris Shaders** - *Native integration for directory navigation inside shader options.*   
    *   **Resourcify** - *Embedded asset tracking directly inside the options layout.*   
    *   **Stack Refill** - *Automatically replaces exhausted resources from backpack reserves.*   
    *   **Visual Workbench** - *Items remain physically dropped inside the crafting grid matrix.*   
    *   **** - **   
    *   **** - **     

    
## **Optimizations**   
*The following mods has been added to improve quality and performance*   
    *   **[TT20](https://curseforge.com)** - *TT20 helps reduce lag by optimizing how ticks work when the server's TPS is low.*   
    *   **[Epic Fight (FPS Optimizer)](https://www.curseforge.com/minecraft/mc-mods/epic-fight-fps-optimizer)** - *A configurable client-side FPS optimizer, reduces distant animation and visual effect rendering costs*   
    *   **[All The Leaks](https://www.curseforge.com/minecraft/mc-mods/alltheleaks)** - *Crash prevention and optimization*   
    *   **Saturn** - *Optimized memory usage and re-mapped memory leak garbage tracking.*   
    *   **Smooth Boot** - *Smooth loading allocations across split core processing.**   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **[AAA Particles](https://www.curseforge.com/minecraft/mc-mods/aaa-particles)** - *Library mod that enables using effekseer particles (.efkefc) in minecraft.*   
    
## **Add-ons**   
*The following mods are add-ons for mods already in the modpack.*   
     *   **[Mekanism Nuclear Weapons & Explosives](https://www.curseforge.com/minecraft/mc-mods/mekanism-nuclear-weapons-explosives)** - *Addon for mekanism that adds nuclear,hydrogen and antimatter bombs*   
    *   **** - **   
    *   **[TacZ Attributes (Addon)](https://www.curseforge.com/minecraft/mc-mods/tacz-attributes-addon)** - **   
    *   **[TacZ: Blueprints Reforged](https://www.curseforge.com/minecraft/mc-mods/tacz-blueprints-reforged)** - *TaCZ: Blueprints Reforged is an addon for TaCZ that turns guns and attachments into something you have to discover and earn.*   
    *   **[TacZ Addon](https://www.curseforge.com/minecraft/mc-mods/tacz-addon)** - *An expansion mod for TaCZ.*   
    *   **[Veil Lights for TacZ](https://www.curseforge.com/minecraft/mc-mods/veil-lights-for-tacz)** - *Addon that renders configured TaCZ weapon lights through the separate Veil Volume Lights library*   
    *   **[Sophisticated Tactical Backpacks](https://www.curseforge.com/minecraft/mc-mods/sophisticated-tactical-backpacks)** - *Add-on for Sophisticated Backpacks that adds military-style camouflage appearance and an Ammo Reload Upgrade that is compatible with several firearm mods (like TacZ).*   
    *   **** - **   
    *   **[Just Enough TacZ](https://www.curseforge.com/minecraft/mc-mods/jet-just-enough-tacz)** - *This mods adds config that allows removal of guns and addons from the game*   
    *   **(IU) Watering Can** - *Farming utility.*   
    *   **** - **   
    *   **** - **   
    
    
## **Integrations**   
*The following mods are integrations to improve various things such as configuration and data*   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    
    
## **Compatibility**
*The following mods has been added to make more mods compatible*   
    *   **Epic Fight Auto Compat** - *Background translation framework for out-of-the-box combat styles.*   
    *   **Epic Tweaks** - *Core adjustments for overall damage parameters and entity behaviors.*   
    *   **Epic Curios Elytra** - *Allows slotting of standard flight parameters inside Curios accessories.*   
    *   **[Epic Fight: Curios Compat 2.0](https://curseforge.com)** - *Adds compatibility/fix between Curios and Curios*   
    *   **[Epic Fight x Punchy](https://curseforge.com)** - *Adds compatibility between Punchy and Epic Fight*   
    *   **[TacZ: Curios](https://www.curseforge.com/minecraft/mc-mods/taczcurios)** - *TaczCurios adds custom curios (accessories) to the mod TacZ*   
    *   **[Mystical Agriculture Compats](https://www.curseforge.com/minecraft/mc-mods/mystical-agriculture-compats)** - *Adds compatibility between Mystical Agriculture, Mekanism's Enrichment Chamber and EnderIO's SAG Mill*   
    *   **[Mystical Engineering](https://www.curseforge.com/minecraft/mc-mods/mystical-engineering)** - *Adds comaptibility between Mystical Agriculturea and Immersive Engineering's "Garden Clocke"*   
    *   **[CIT Resewn](https://www.curseforge.com/minecraft/mc-mods/cit-resewn)** - *Re-implements MCPatcher's CIT*   
    *   **[CITResewnNeoPatcher](https://www.curseforge.com/minecraft/mc-mods/cit-resewn-neopatcher)** - *Patches CIT Resewn mods so it runs on NeoForge through Sinytra Connector*   
    *   **BetterEnd x Chipped** - *Massive expansion of decorative variant choices for End-materials.*   
    *   **[Iris Veil Compat](https://www.curseforge.com/minecraft/mc-mods/iris-veil-compat)** - *Allow mods using the Veil rendering engine to render correctly when using Iris shaderpacks.*
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    
  
## **Misc**   
*Libraries, engines and more requires mods*   
    *   **[CreativeCore](https://www.curseforge.com/minecraft/mc-mods/creativecore)** - *Core for LittleTiles*   
    *   **[MezzConfig](https://www.curseforge.com/minecraft/mc-mods/mezzconfig)** - *Simple configuration library for mods*   
    *   **Toadlib** - *Core foundation engine for updated asset rendering blocks.*   
    *   **[Veil Volume Lights](https://www.curseforge.com/minecraft/mc-mods/veil-volume-lights)** - *Veil addon library that adds support for colored mediums.*   
    *   **[Apothic Attributes](https://www.curseforge.com/minecraft/mc-mods/apothic-attributes)** - *A library mod providing Attributes and related things*    
    *   **Eating Animation (Core)** - *Restores fundamental consumption mechanics for base items.*   
    *   **[KubeJS](https://www.curseforge.com/minecraft/mc-mods/kubejs)** - *for workking on upcoming features*   
    *keybinds
    *   **[KubeJS Additions](https://www.curseforge.com/minecraft/mc-mods/kubejs-additions)** - *for workking on upcoming features*   
    *geckoJS   
    *KJS Editor   
    *questJS   
    *   **[KubeJS Mekanism](https://www.curseforge.com/minecraft/mc-mods/kubejs-mekanism)** - *for workking on upcoming features*   
    *mekanism extend    
    *   **[KubeJS Curios](https://www.curseforge.com/minecraft/mc-mods/kubejs-curios)** - *for workking on upcoming features*   
    *   **[KubeJS EnderIO](https://www.curseforge.com/minecraft/mc-mods/kubejs-enderio)** - *for workking on upcoming features*   
    *   **[KubeJS LootJS](https://www.curseforge.com/minecraft/mc-mods/lootjs)** - *for workking on upcoming features*   
    *   **[KubeJS Occultism](https://www.curseforge.com/minecraft/mc-mods/occultism-kubejs)** - *for workking on upcoming features*   
    *   **[KubeJS Ars Nouveau](https://www.curseforge.com/minecraft/mc-mods/kubejs-ars-nouveau)** - *for working on upcoming features*   
    *   **[KubeJS Draconic Evolution](https://www.curseforge.com/minecraft/mc-mods/kubejs-draconic-evolution)** - *for working on upcoming features*   
    *   **[KubeJS ProjectE](https://www.curseforge.com/minecraft/mc-mods/kubejs-projecte)** - *for working on upcoming features*   
    *   **[KubeJS Applied](https://www.curseforge.com/minecraft/mc-mods/applied-kubejs-kjs-ae2)** - *for working on upcoming features*   
    *Custom meteor   
    *neo   
    *IU   
    *rechisled   
    *Immersive E   
    *   
    *FTB Library   
    *FTB Quests   
    *FTB Quests enhance   
    *FTB Quest Quick Check    
    *FTB Quest Optimizer   
    *FTB Quest Entity Visualization   
    *FTB Extra Quests   
    *FTB Quest Completion Broadcast   
    *FTB Teams   
    *   
    *Extra quests   
    *PlayerNBT   
    *Progressive Stages   
    *UI Quests   
    *Certain Question additions   
    *   
    *   **GroovyModLoader (GML)** - *Lower-level backend optimization for early mod setup strings.*   
    *   **Loot Integrations** - *Implemented global looting balance patches covering *Born in Chaos, Cataclysm, Integrated, Yung's, and Vanilla* variables.*   
    *   **Reactor Plus** - *Advanced custom coolant channels and higher energy tiering modules*.   
    *   
    *   **Cupboard** - **   
    *   **[ForgeEndertech](https://www.curseforge.com/minecraft/mc-mods/forgeendertech)** - *Core library for `Large Ore Deposits`, `Advanced Hook Launchers` and `Advanced Finders`*   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
    *   **** - **   
     

---

## 🔄 Mod Updates & Removals   

##**Updated:**   
     *   **CITResewnPatcher** -> Updated from Fabric version *(ran with Sinytra Connector)* to [NeoForge version](https://www.curseforge.com/minecraft/mc-mods/cit-resewn-neopatcher)   
     *   **[AE2 Growth Accelerator Tiers](https://www.curseforge.com/minecraft/mc-mods/ae2-growth-accelerators)** -> Updated to `AGA Neo 1.21.1 2.2.0`   
     *   **Applied Pneumatics** -> Updated from `1.0.8` to `1.0.9`   
     *   **Ars QOL** -> Updated from `1.0.0` to `1.1.0`   
     *   **AutoEMC** -> Updated from `2.1.0` to `2.1.1`   
     *   **Balm** -> Updated from `21.0.65` to `21.0.66`   
     *   **CBCAT Fix** -> Updated from `1.1.0` to `1.1.2`   
     *   **CIT Resewn** -> Updated to `patched_citresewn-1.2.2+1.21.jar`   
     *   **CompatLink** -> Updated from `1.1.2` to `1.3.0`   
     *   **Create Compression** -> Updated from `2.0.0` to `2.0.1`   
     *   **Create: Lazy Tick** -> Updated from `2.6.25-6.0.10` to `2.7.29-6.0.10`   
     *   **Display Delight** -> Updated from `1.6.0` to `1.7.0`   
     *   **Distraction Free Recipes** -> Updated from `1.2.1` to `1.2.2`   
     *   **Enderite Mod** -> Updated from `1.6.2` to stable `1.6.1`   
     *   **Extreme Reactors** -> Massive backend update from `2.4.9` to `2.4.28`   
     *   **Fight Back** -> Updated from `1.3.0` to `1.3.2`   
     *   **Industrial Upgrade** -> Updated from `3.4.0.11` to `3.4.0.13`   
     *   **Interiors (Macaw's Create)** -> Updated to `interiors-0.6.1 v2.jar`   
     *   **Ksyxis** -> Updated from `1.4.4` to `1.4.5`   
     *   **LittleTiles** -> Updated from `1.6.0-pre229` to `1.6.0-pre230`   
     *   **Zelda: Legend of the Master Sword** -> Updated from `2.4.2` to `2.4.6`   
     *   **Mekanism Turrets** -> Updated from `2.2.2` to `2.2.3`   
     *   **Mekanism Unleashed** -> Updated from `0.3.2` to `0.3.4`   
     *   **Mekanism TrashCube** -> Updated from `2.0.4-NeoForge` to `2.0.5-NeoForge`   
     *   **More Backpack Upgrades** -> Updated from `1.0.5` to `1.0.7`   
     *   **Modonomicon** -> Updated from `1.120.5` to `1.120.7`   
     *   **Moonlight Lib** -> Updated from `3.6.8` to `3.6.9`   
     *   **Neo Vitae** -> Updated from `1.1.26` to `1.1.27`    
     *   **Polytone** -> Updated from `4.5.0` to `4.5.1`   
     *   **Power Utilities** -> Updated from `1.3` to `1.5`    
     *   **Quantum Generators** -> Updated from `1.4` to `1.5`   
     *   **Simply Quarries** -> Updated from `1.3` to `1.4`   
     *   **TaczCurios (TCC)** -> Updated from `1.4.1+1.21.1` to `1.4.1-hotfix+1.21.1`   
     *   **The Ravenous** -> Major jump from version `2.0.5` to `3.0`   
     *   **Tooltip Overhaul** -> Updated from `2.0.3` to `2.0.4`   
     *   **Valhelsia Core** -> Updated from `1.1.4` to `1.1.5`   
     *   **Veil** -> Updated from `4.5.0` to `4.5.1`   
     *   **Waystones** -> Updated from `21.1.45` to `21.1.46`   
     *   **Yukami's Sophisticated Backpack Tab** -> Updated from `2.1.1` to `2.2.0`   
     *   **Zero CORE 2** -> Updated from `2.4.9` to `2.4.21`   


### **Mod Removals:**   
*Due to incompatibilities, change of vision and more, we've decided to remove the following mods from this version:*   
    *   **[Distant Horizons](https://www.curseforge.com/minecraft/mc-mods/distant-horizons):** *Replaced by Voxy*   
    *   **Every Compat - "[Wood Good](https://www.curseforge.com/minecraft/mc-mods/every-compat)", "[Stone Zone](https://www.curseforge.com/minecraft/mc-mods/stone-zone)", "[Gems Realm](https://www.curseforge.com/minecraft/mc-mods/gems-realm)":** *Removed for now because incompatibility, and other mods like `Almost Unified` cover most of this anyway.*   
    *   **Create Blocks & Bogies:** *Extracted to preserve clean schematic layouts in custom factory builds.*   
    *   **Just Enough Items (JEI):** *Swapped out to optimize full item directory syncing over heavy modpack networks.*   
    *   **Mekanism: Elements:** *Purged from the environment chain to prevent recipe conflicts with advanced alloy automation.*     
    *   **Sophisticated JEI Index:** *Legacy tracking indexing, no longer needed under the streamlined directory overhaul.*   
    *   **AE2 Lightning Tech:** *Outdated version and it's "a bit too much"*   
    *   **AE2: Better Villagers:** *Causing fatal `MenuType` error*   
    *   **Create: Better Villagers:** *Causing fatal `MenuType` error*   
    * **Remove Loading Screen:** The mod [Remove loading screen](https://modrinth.com) has been permanently removed from the pack *(removed in v0.1.2-alpha-r.dev)*, as it is **completely** incompatible with our   
<details>
<summary>upcoming..</summary>   
    
* **[Fancy Menu](https://modrinth.com)** UI setup.   
    * Fully customized main menu, "ESC" menu, video settings, audio settings etc.   
* **Drippy Loading Screen**   
    * Fully customized loading screen   
* **Fully customized music in menus**   
</details>   

---

# 🗺️ **ROADMAP**   

## Mods to be added:   
   *   **[Ancient Remnants: Monoliths](https://www.curseforge.com/minecraft/mc-mods/ancient-remnants)** - *waiting on 1.21.1 version*   
   *Discover mysterious monoliths and uncover the ancient powers hidden within!*   
   *   
   *   
   *   
   *   

## Changes   

We're going to start focusing a bit more on various custom changes using KubeJS, Integration, Pachouli and other related configs etc. as well as quality changes for balancing, quests and atmosphere; like the FancyMenu changes I mentioned in "Removed" above to keep the "creepy" horror-like feeling relevant.   
We will also be making it harder to access certain items *(like powerful guns and spells)* to balance the progression and make it feel like you're really trying to "evolve" and enhance your knowledge to be on par with the dark entities that haunt you.   


---

# Known Issues:   
**[Here](https://github.com/ImFloofo7/thelastcircuit/blob/v0.2.0/troubleshooting%20and%20knows%20issues.md)** you can find known issues regarding this version and on how to fix *most* of them.   

---
## ⚠️ IMPORTANT DISCLAIMER (Please Read)   
This release marks our definitive transition to the CurseForge architecture.     
***Ensure your old Modrinth profiles are fully backup-archived before deploying this package***.    
Manual file transfers of older development branches **(v0.1.0-alpha-r.dev)** into this environment *may* corrupt your script directories and trigger hard boot errors.

***Thank you to all our Closed alpha testers for sifting through crash logs and helping us bring the pack to a better, more optimized bootable state! Please report any freezes, bugs or exploits in our dedicated Discord channels.***   












