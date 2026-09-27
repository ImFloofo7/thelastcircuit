# **WORK IN PROGRESS**


# 🛠️ Changelog: v0.2.0-alpha

### [Epic Fight "Nightfall"](https://curseforge.com) & [GabouLibs](https://curseforge.com) now included!
Managed to come to an agreement on permission of usage for the mods, so they are now included in the modpack!

**HUGE** Thanks to [Gaboouu](https://github.com) & ["Super_awespme_baby"](https://curseforge.com) again for granting me permission to include these in the modpack! ❤️

### Platform changes!
In the requirements of getting permission for said mods were to publish on CurseForge. Together with some technical reasons amongst other, we've decided to switch to CurseForge permanently!
*(Project on Modrinth has been deleted and **v0.1.0-alpha-r.dev** is no longer available for the public).*

***Please note: we do not condone in republishing this modpack without the permission from the author of this modpack anymore.***
*(Please see updated [license](https://github.com))*

---

## ⚙️ Optimizations & Fixes
* **Cleaned Up Glas Codes:** Fixed fatal JSON metadata boot errors (`No key pack_format`) hidden inside the customized resource packs.
* **Launch Performance:** Fixed early launch loading stalls and graphics adapter workarounds by purging legacy translation caches.
* **Engine Optimizations:** Enhanced thread prioritization and sub-millisecond memory cleanups (`ZGC`) to completely eliminate cyclic lag spikes in heavy factory zones.

---

## 🎨 Resource Pack Architecture

To make things as seamless as possible for alpha testing, a massive overhaul has been done to the Resource Pack system. All custom assets, dark UI themes, and Fresh Animations patches are now **fully numbered and categorized in their strict logical loading order**.

If the game layout resets or doesn't load them automatically on your first boot, simply move them into the active (`Selected`) column and stack them following their prefix indices:

1. **👑 UI, Fonts & Fixes (Absolute Top):** Everything starting with `.4.1.x` - Activates the true dark interface overlays, custom tooltips, and hotbar boundaries.
2. **🧬 Custom Models & Entities:** Everything starting with `.3.2.x` - Loads the main Fresh Animations core engine first, followed directly by its official extensions (`FA+`) and third-party entity compatibility patches.
3. **⚔️ Mod Add-ons & Patches:** Everything starting with `.2.1.x` - Specific compatibility patches linking modified tech blocks and specialized item actions (like Eating Animations).
4. **🧱 Base / Overhaul Texture Packs (Absolute Bottom):** Everything starting with `.1.1.x` - The high-resolution Faithful 64x base models forming the foundational textures of the entire world.

---

## 🔄 Mod Updates & Removals

### **Mod Updates & Added:**

* **Updated:**
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

* **Added:**
     *   [Epic Fight: Curios Compat 2.0](https://curseforge.com) - Improved compatibility
     *   [TT20](https://curseforge.com) - Improved Performance
            *TT20 helps reduce lag by optimizing how ticks work when the server's TPS is low.*
     *   [Epic Fight x Punchy](https://curseforge.com) - Improved Compatibility
     *   [Bosses'Rise - Epic Fight](https://curseforge.com) - Enhanced animations for customized boss configurations.
     *   **Advanced Peripherals** - *Expands ComputerCraft setup with advanced technical interactions.*
     *   **BetterEnd Cities** - *Generates unique city structures and progression markers throughout the End dimension.*
     *   **BetterF3 Spark Module** - *Directly links hardware monitoring with the F3 menu interface.*
     *   **Bio-Scanner** - *Faction tracking and specialized entity identification.*
     *   **CC: Tweaked** - *Full automation and programming terminals brought to the tech layout.*
     *   **Chipped (BetterEnd Addon)** - *Massive expansion of decorative variant choices for End-materials.*
     *   **Diamond Vein** - *Mining optimizations and automated scanning adjustments.*
     *   **Eating Animation (Core)** - *Restores fundamental consumption mechanics for base items.*
     *   **Epic Fight Auto Compat** - *Background translation framework for out-of-the-box combat styles.*
     *   **Epic Fight x Iron's Spells 'n Mobs** - *Links combat engine with complex spellcasting structures.*
     *   **Epic Tweaks** - *Core adjustments for overall damage parameters and entity behaviors.*
     *   **Epic Curios Elytra** - *Allows slotting of standard flight parameters inside Curios accessories.*
     *   **FancyMods BetterEnd Tweaks** - *Balance adjustments and biome-specific block variants.*
     *   **GroovyModLoader (GML)** - *Lower-level backend optimization for early mod setup strings.*
     *   **KubeJS Additions** - *Deep integration for heavily modified server recipe overrides.*
     *   **Loot Integrations (Suite)** - *Implemented global looting balance patches covering *Born in Chaos, Cataclysm, Integrated, Yung's, and Vanilla* variables.*
     *   **Make It Compatible (Voxy)** - *Advanced multi-threaded chunk rendering and visual fixes.*
     *   **Occultism KubeJS** - *Scripting engine control over advanced ritual data structures.*
     *   **Quick Pack** - *Inventory management macro hotkeys.*
     *   **Reactor Plus** - *Advanced custom coolant channels and higher energy tiering modules*.
     *   **Resourcify** - *Embedded asset tracking directly inside the options layout.*
     *   **Roxy Library** - *Mandatory codebase required for early environment setups.*
     *   **Saturn** - *Optimized memory usage and re-mapped memory leak garbage tracking.*
     *   **Search for Iris Shaders** - *Native integration for directory navigation inside shader options.*
     *   **Smooth Boot** - *Smooth loading allocations across split core processing.*
     *   **Stack Refill** - *Automatically replaces exhausted resources from backpack reserves.*
     *   **Toadlib** - *Core foundation engine for updated asset rendering blocks.*
     *   **Tools+** - *High-tier utility tools integrated within technical blueprints.*
     *   **Verity** - *Verification frameworks protecting against data generation mismatches.*
     *   **Visual Workbench** - *Items remain physically dropped inside the crafting grid matrix.*
     *   **Watering Can** - *Farming utility.*
     *   **[All The Leaks](https://www.curseforge.com/minecraft/mc-mods/alltheleaks)** - *Crash prevention and optimization*
     *   **Cupboard** - **
     *   **AAA Particles** *(+ AAA World)* - **
     *   **[Laser IO](https://www.curseforge.com/minecraft/mc-mods/laserio)** - *EnderIO Pipes but reworked and additional content*

### **Mod Removals:**
Due to incompatibilities, change of vision and more, we've decided to remove the following mods from this version:

* **Remove Loading Screen (Removed):** The mod `[Remove loading screen](https://modrinth.com)` has been permanently removed from the pack *(removed in v0.1.2-alpha-r.dev)*, as it is **completely** incompatible with our 
<details>
<summary>upcoming..</summary>   
     * **[Fancy Menu](https://modrinth.com)** UI setup.
          * Fully customized main menu, "ESC" menu, video settings, audio settings etc.
     * **Drippy Loading Screen**
          * Fully customized loading screen
     * **Fully customized music in menus**
</details>   
    *   **Applied KubeJS (`applied_kjs`):** *Removed due to script conflicts with newer technical asset loaders.*
    *   **Create Blocks & Bogies (create_bb):** *Extracted to preserve clean schematic layouts in custom factory builds.*
    *   **Just Enough Items (jei):** *Swapped out to optimize full item directory syncing over heavy modpack networks.*
    *   **Mekanism: Elements (mekanismelements):** *Purged from the environment chain to prevent recipe conflicts with advanced alloy automation.*
    *   **Sophisticated JEI Index (sophisticated_jei_index):** *Legacy tracking indexing, no longer needed under the streamlined directory overhaul.*
    *   **AE2 Lightning Tech:** Outdated version
    
##⚠️ IMPORTANT DISCLAIMER (Please Read)
This release marks our definitive transition to the CurseForge architecture.    
***Ensure your old Modrinth profiles are fully backup-archived before deploying this package***.    
Manual file transfers of older development branches **(v0.1.0-alpha-r.dev)** into this environment *may* corrupt your script directories and trigger hard boot errors.

***Thank you to all our Closed alpha testers for sifting through crash logs and helping us bring the pack to a better, more optimized bootable state! Please report any freezes, bugs or exploits in our dedicated Discord channels.***












