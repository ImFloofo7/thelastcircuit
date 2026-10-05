# **WORK IN PROGRESS**

<img width="2172" height="724" alt="TCL Banner Alt compressed" src="https://github.com/user-attachments/assets/d0b1f9dc-5e09-4c53-bc24-1944512ae51c" />


# V0.2.0-Alpha IS HERE, **AND IT'S HUGE!**

# 🛠️ Changelog: v0.2.0-alpha

### ☑️ Mod permissions!


### [Epic Fight-Nightfall](https://www.curseforge.com/minecraft/mc-mods/epicfight-nightfall) & [Gabou's Libs](https://www.curseforge.com/minecraft/mc-mods/gabous-libs) now included!

Finally managed to come to an agreement on permission of usage for the mods, so they are now included in the modpack!

**HUGE THANKS** to **[Gaboouu](https://www.curseforge.com/members/gaboouu/projects)** & **[Super_awespme_baby](https://www.curseforge.com/members/super_awesome_baby/projects)** again for granting me permission to include these in the modpack! ❤️


### 🆕 Major **NEW** Additions!

**[Voxy](https://github.com/NHblock-Johnsnow/neo-voxy-multiversion)** - *New LoD rendering mod*   
   
We have **ALSO** decided to switch over to ***Voxy*** for many reasons.    
Unfortunately, until [MCRcortex](https://github.com/MCRcortex/) makes an official back-port, you will have to install it manually ***(see steps below)*** since I am **not** allowed to distribute any actual files.   


<details>
<summary>How to Install Voxy</summary>

**1.** Go to the GitHub for the [unofficial backport](https://github.com/NHblock-Johnsnow/neo-voxy-multiversion).   
**2.** Clone or download the source code/zip to your computer.   
3**.** Build the project using Gradle, VSCode or IntelliJ. 
      *(If you want to use an IDE instead of the terminal, you can follow these video tutorials:)*      
         • Video Guide: [How to build Gradle projects with VS Code](https://www.youtube.com/watch?v=Y6Qd_Bovo-o)
         • Video Guide: [How to build Gradle projects with IntelliJ IDEA](https://www.youtube.com/watch?v=e500ohACgYI&xstg=CAMSEBUJ_b-oH-PhF0yjBgavkzY%3D)
         • *Alternatively, you can follow this text-based Reddit Guide: [How to get Voxy running on NeoForge 1.21.1](https://www.reddit.com/r/feedthebeast/comments/1sl0xp4/guide_how_to_get_voxy_running_on_neoforge_1211/), though you should use **[THIS VERSION](https://github.com/NHblock-Johnsnow/neo-voxy-multiversion)**, **NOT** the version provided in the reddit guide. *([version](https://github.com/m3t4f1v3/voxy/tree/mc_1211)**
         
**4.** Once the build is finished, grab the generated `.jar` file from the "`build`/`libs`*" folder and move it into the  Minecraft mods folder ([1:14](https://www.youtube.com/shorts/TvEFK4pbVEE?t=75)).   
***(Normally located in;** [DRIVE LETTER]:\Users\[USER]\curseforge\minecraft\Instances\The Last Circuit v`x.x.x-x`)*   
   
***Please note that this is an unofficial community version***, so you **cannot** get official support from [MCRcortex](https://github.com/MCRcortex/) if you encounter any bugs.***  
*Please report potential bugs on the discord - linked at the bottom of this page.*
</details>


### 🔄 Platform changes!
One of the requirements for getting permission to include Nightfall and [Gabou's Libs](https://www.curseforge.com/minecraft/mc-mods/gabous-libs) was that we publish on CurseForge. Combined with a few technical reasons, we have decided to switch to CurseForge **permanently**!
*(Project on Modrinth has been deleted and **`v0.1.0-alpha-r.dev`-`v0.1.9-alpha-r.dev`** is no longer available for the public).*



***Please note: we do not condone in republishing this modpack without the permission from the author of this modpack anymore.***
*(Please see updated [license]([https://github.com](https://github.com/ImFloofo7/thelastcircuit/blob/Latest/LICENSE.md)))*

---

## ⚙️ Optimizations & Fixes
<details>
  <summary>Optimizations</summary>   

  * **Launch Performance:** Fixed early launch loading stalls and graphics adapter workarounds by purging legacy translation caches.   
  * **Engine Optimizations:** Enhanced thread prioritization and sub-millisecond memory cleanups *("`ZGC`")* to completely eliminate cyclic lag spikes in heavy factory zones.   
  * **Optimized overall performance:** We've optimized the pack to run smoother thanks to: 
     *   Removing mods
     *   Adding *more* compatibility- and performance mods
     *   Making some configurations to utilize said mods   
</details>
  
<details>
<summary>Fixes & QoL</summary>
  
  * **Cleaned Up Codes:** Fixed multiple fatal JSON metadata boot errors *(like "`No key pack_format`")* hidden inside the 
  resource packs.
  * **[Managed order for resourcepacks](https://github.com/ImFloofo7/thelastcircuit/edit/v0.2.0/Changelog%20v0.2.0-alpha.md#-resource-pack-architecture):** Custom order for resource packs

</details>


***We're constantly working on making the modpack run smoother on all systems, though it is hard for lower-end systems because of the size of this modpack, so we kindly ask you to bare with us.***



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
*Start with adding **`0.1.1`** first, **`0.1.2`** second, etc.*

***Disclaimer!***
Some resourcepacks are built-in with some mods and should be left at the bottom of the loading order, except for "punchy" which should be placed between `1.3.27` and `2.1.1`

---

## 🖥️ MOD updates, removals and added.


<details>
  <summary>▶️ Added:</summary>
    <details>
    <summary>New Features & Core Content</summary> 
      
  ***The following mods are new additions to the modpack that make changes to one thing or another.***    
  *   **[ProgressiveStages](https://www.curseforge.com/minecraft/mc-mods/progressivestages)** - *Adds a progression system in-game, this will be used for the main "**Questline**" that is under development.*
  *   **[Laser IO](https://www.curseforge.com/minecraft/mc-mods/laserio)** - *EnderIO Pipes but reworked, and with additional content.*   
  *   **[TacZ: AoS](https://www.curseforge.com/minecraft/mc-mods/tacz-art-of-sniping)** - *TACZ: AoS lets you snipe entities from extreme distances with realistic ballistics.*   
  *   **[Epic Fight - Bosses'Rise](https://www.curseforge.com/minecraft/mc-mods/bossesrise)** - *Adds souls-like bosses, dungeons and loot.*   
  *   **BetterEnd Cities** - *Generates unique city structures and progression markers throughout the End dimension.*   
  *   **Bio-Scanner** - *Faction tracking and specialized entity identification.*   
  *   **[TacZ Attributes](https://www.curseforge.com/minecraft/mc-mods/tacz-attributes)** - *Adds more than 250 attributes to TacZ weapons*   
  *   **[LittleTiles](https://www.curseforge.com/minecraft/mc-mods/littletiles)** - *Adds the ability to create micro (pixel) blocks.*   
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
    </details>

  <details>
    <summary>QoL</summary>

***Small mods that doesn't really add any "new content", but are still nice to have.***    
  *   **[Voxy](https://github.com/NHblock-Johnsnow/neo-voxy-multiversion)** - *A Minecraft LoD rendering mod, letting you to render hundreds of chunks with little to no performance impact*
  *   **[Roxy](https://www.curseforge.com/minecraft/mc-mods/roxy)** - *Allows Voxy (that is for fabric) to work on NeoForge*
  *   **[SeeU](https://www.curseforge.com/minecraft/mc-mods/seeu)** - *Makes distant players visible far beyond canilla entity tracking, Compatible with Voxy*
  *   **[Thunderhead](https://www.curseforge.com/minecraft/mc-mods/thunderhead)** - *Lightning & Thunder overhaul.*
  *   **[AAA Particles](https://www.curseforge.com/minecraft/mc-mods/aaa-particles)** - *Library mod that enables using effekseer particles (.efkefc) in minecraft.*
  *   **AAA World** - **
  *    **[Punchy!](https://www.curseforge.com/minecraft/mc-mods/punchy)** - *Engine for various first-person animations.*
  *   **[Quick Pack](https://www.curseforge.com/minecraft/mc-mods/quick-pack)** - *Improves datapack & resourcepack zip gile loading times.*   

  
  *   **BetterF3 Spark Module** - *Addon for Directly links hardware monitoring with the F3 menu interface.*       

        
     
 
   
  *   **FancyMods BetterEnd Tweaks** - *Balance adjustments and biome-specific block variants.*   
  *   **Search for Iris Shaders** - *Native integration for directory navigation inside shader options.*   
  *   **Resourcify** - *Embedded asset tracking directly inside the options layout.*   
  *   **Stack Refill** - *Automatically replaces exhausted resources from backpack reserves.*   
  *   **Visual Workbench** - *Items remain physically dropped inside the crafting grid matrix.*   
  *   **** - **   
  *   **** - **     
    </details>
    
  <details>
    <summary>Optimization mods</summary>
   
***The following mods has been added to improve quality and performance***   
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
   
</details>

<details>
    <summary>Add-ons</summary>    
 
***The following mods are add-ons for mods already in the modpack.***   
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
    </details>

<details>
    <summary>Integrations</summary>
  
*The following mods are integrations to improve various things such as configuration and data*   
  *   **** - **   
  *   **** - **    
  *   **** - **
  *   **** - **   
  *   **** - **    
  *   **** - **   
    </details>

<details>
    <summary>Compatibility</summary>    

***The following mods has been added to make more mods compatible***   
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
    </details> 

<details>
    <summary>Misc</summary>  

***Libraries, engines and more requires mods***   
  *   **[CreativeCore](https://www.curseforge.com/minecraft/mc-mods/creativecore)** - *Core for LittleTiles*   
  *   **[MezzConfig](https://www.curseforge.com/minecraft/mc-mods/mezzconfig)** - *Simple configuration library for mods*   
  *   **Toadlib** - *Core foundation engine for updated asset rendering blocks.*   
  *   **[Veil Volume Lights](https://www.curseforge.com/minecraft/mc-mods/veil-volume-lights)** - *Veil addon library that adds support for colored mediums.*   
  *   **[Apothic Attributes](https://www.curseforge.com/minecraft/mc-mods/apothic-attributes)** - *A library mod providing Attributes and related things*    
  *   **[Eating Animation (Core)](https://www.curseforge.com/minecraft/mc-mods/eating-animation-forge)** - *Restores fundamental consumption mechanics for base items.*   
  *   **[KubeJS](https://www.curseforge.com/minecraft/mc-mods/kubejs)** - *for workking on upcoming features*   
  *keybinds
  *   **[KubeJS Additions](https://www.curseforge.com/minecraft/mc-mods/kubejs-additions)** - *for workking on upcoming features*  
  *    **[KubeJS Applied](https://www.curseforge.com/minecraft/mc-mods/applied-kubejs-kjs-ae2)** - *for working on upcoming features*   
  *   **[KubeJS Ars Nouveau](https://www.curseforge.com/minecraft/mc-mods/kubejs-ars-nouveau)** - *for working on upcoming features*  
  *   **[KubeJS Create](https://www.curseforge.com/minecraft/mc-mods/kubejs-create)** - *Create integration for KubeJS - **for upcoming changes***
  *   **[KubeJS Curios](https://www.curseforge.com/minecraft/mc-mods/kubejs-curios)** - *for workking on upcoming features*  
  *   **[KubeJS CustomMeteor](https://www.curseforge.com/minecraft/mc-mods/custommeteorjs)** - *AE2 addon for modpack makers. It lets you control meteorite blocks and terrain behavior without editing AE2 itself.*
  *   **[KubeJS Draconic Evolution](https://www.curseforge.com/minecraft/mc-mods/kubejs-draconic-evolution)** - *for working on upcoming features*
  *   **[KubeJS EnderIO](https://www.curseforge.com/minecraft/mc-mods/kubejs-enderio)** - *for workking on upcoming features*     
  *  *geckoJS   
  *KJS Editor      
  *   **[KubeJS Mekanism](https://www.curseforge.com/minecraft/mc-mods/kubejs-mekanism)** - *for workking on upcoming features*   
 
  *   **[KubeJS Mekanism extends](https://www.curseforge.com/minecraft/mc-mods/kubejs-mekanism-extends)** - *for workking on upcoming features*    


  *   **[KubeJS LootJS](https://www.curseforge.com/minecraft/mc-mods/lootjs)** - *for workking on upcoming features*   
  *   **[KubeJS Occultism](https://www.curseforge.com/minecraft/mc-mods/occultism-kubejs)** - *for workking on upcoming features*   
   
     
  *   **[KubeJS ProjectE](https://www.curseforge.com/minecraft/mc-mods/kubejs-projecte)** - *for working on upcoming features*   
  
  *   **[QuestJS](https://www.curseforge.com/minecraft/mc-mods/questjs)** - *FTB Quests KubeJS Events adds client-side KubeJS events for the FTB Quests GUI.*
  
  ** neo**   
  ** IU **   
  **rechisled**   
  **Immersive E**   
  **KubeJS Keybinds**   
  *   **[FTB Library](https://www.curseforge.com/minecraft/mc-mods/ftb-library-forge)** - *Library for FTB Quests.*   
  *   **[FTB Teams](https://www.curseforge.com/minecraft/mc-mods/ftb-teams-forge)** - *Library for mods that can utilize team progression like FTB Chunks and FTB Quests.*   
  *   **[FTB Quests](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-forge)** - *Quest book system*
  *   **[FTB Quests enhance](https://www.curseforge.com/minecraft/mc-mods/quest-enhance)** - *Client-side "enhancement" mod        for FTB Quests*   
  *   **[FTB Quest Quick Check](https://www.curseforge.com/minecraft/mc-mods/ftb-quest-quick-check)** - *FTB Quest Quick             Check adds a button to the FTB Quests GUI that completes all currently available checkmark tasks in one action.*   
  *   **[FTB Quest Optimizer](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-optimizer)** - *Removes micro-freezes when moving items and turning in quests, makes inventory checking smarter and quieter for the server*   
  *   **[FTB Quest Entity Visualization](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-entity-visualization)** -           *This mod replaces the boring spawn‑egg icon in a kill task with the actual entity rendered live in 3D.*   
  *   **[FTB Extra Quests](https://www.curseforge.com/minecraft/mc-mods/extraquests)** - *Addon adds new tasks, rewards and functions*   
  *   **[FTB Quest Completion Broadcast](https://www.curseforge.com/minecraft/mc-mods/quest-completion-broadcast)** - *Chat announcements for quest, (including for players on other teams).*        
  *   **[PlayerNBT Quests](https://www.curseforge.com/minecraft/mc-mods/playernbt-quests-ftb-quests)** - *Extension mod that provides quest creators with player NBT data detection functionality. *   
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
    </details>     
</details>

---

## 🔄Mod Updates & Removals   

<details>
  <summary>Updated</summary>
  
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
</details>

<details>
  <summary>Removed</summary>  
  
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
</details>

---

# 🗺️ **ROADMAP**   

***This is the roadmap for v0.3.0-alpha.***

## Mods to be added:   
   We're constantly looking at adding and removing mods until we're satisfied with the pack, here are some mods we plan to add in the future:
   *   **[Ancient Remnants: Monoliths](https://www.curseforge.com/minecraft/mc-mods/ancient-remnants)** - *waiting on 1.21.1 version*   
   *Discover mysterious monoliths and uncover the ancient powers hidden within!*   

---

## Configurations and Custom content:
### Changes   

We're going to start focusing a bit more on various custom changes using 
  * KubeJS 
  * various "integrations"
  * Pachouli
  * FTB Quests 
and other related configs etc. 

But also quality changes for balancing, quests and atmospheric changes and improvement.   
Like the FancyMenu changes I mentioned [here](https://github.com/ImFloofo7/thelastcircuit/blob/v0.2.0/Changelog%20v0.2.0-alpha.md#mod-updates--removals:~:text=error-,Remove,menus), to keep the "creepy" horror-like feeling relevant throughout the whole pack.   
We will also be making it "*harder*" to access certain items *(like powerful guns and spells)*, implementing a **immersive progression system** to balance the modpack and actually make you work to stay alive, using [FTB Quests](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-forge) and [Progression Stages](https://www.curseforge.com/minecraft/mc-mods/progressivestages)    


### If you want more sneak peeks, I highly recommend you..
<a href="http://discord.gg/A3TFF6TqEU" title="Redirects to The Last Circuit discord">
  <img width="500" height="175" alt="JoinOurDiscord" src="https://github.com/user-attachments/assets/54c6a0cc-b757-4fa7-af55-bee608a78be9" />
</a>



---

# Known Issues:   
**[Here](https://github.com/ImFloofo7/thelastcircuit/blob/v0.2.0/troubleshooting%20and%20knows%20issues.md)** you can find known issues regarding this version and on how to fix *most* of them.   

---

## ⚠️ IMPORTANT DISCLAIMER *(Please Read)*

### ***[LICENSE](https://github.com/ImFloofo7/thelastcircuit/blob/Latest/LICENSE.md) HAS BEEN UPDATED.***
This release marks our definitive transition to the CurseForge architecture.     
***Ensure your old Modrinth profiles are fully backup-archived before deploying this package***.    
Manual file transfers of older development branches **(v0.1.0-alpha-r.dev)** into this environment *may* corrupt your script directories and trigger hard boot errors.

***Thank you to all our Closed alpha testers for sifting through crash logs and helping us bring the pack to a better, more optimized bootable state! Please report any freezes, bugs or exploits in our dedicated Discord channels.***   












