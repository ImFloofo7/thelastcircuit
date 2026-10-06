# **WORK IN PROGRESS**

***Banner coming soon***


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
**3.** Build the project using Gradle, VSCode or IntelliJ. 
      *(If you want to use an IDE instead of the terminal, you can follow these video tutorials:)*      
         • **Video Guide:** *[How to build Gradle projects with VS Code](https://www.youtube.com/watch?v=Y6Qd_Bovo-o)*   
         • **Video Guide:** *[How to build Gradle projects with IntelliJ IDEA](https://www.youtube.com/watch?v=e500ohACgYI&xstg=CAMSEBUJ_b-oH-PhF0yjBgavkzY%3D)*   
         • *Alternatively, you can follow this text-based Reddit Guide: [How to get Voxy running on NeoForge 1.21.1](https://www.reddit.com/r/feedthebeast/comments/1sl0xp4/guide_how_to_get_voxy_running_on_neoforge_1211/), though you should use **[THIS VERSION](https://github.com/NHblock-Johnsnow/neo-voxy-multiversion)**, **NOT** the version provided in the reddit guide. *([version](https://github.com/m3t4f1v3/voxy/tree/mc_1211))**   
         
**4.** Once the build is finished, grab the generated `.jar` file from the "`build`/`libs`*" folder and move it into the  Minecraft mods folder ([1:14](https://www.youtube.com/shorts/TvEFK4pbVEE?t=75)).   
***(Normally located in;** [DRIVE LETTER]:\Users\[USER]\curseforge\minecraft\Instances\The Last Circuit v`x.x.x-x`)*   
   
***Please note that this is an unofficial community version***, so you **cannot** get official support from [MCRcortex](https://github.com/MCRcortex/) if you encounter any bugs.***   
*Please report potential bugs on the discord - linked at the bottom of this page.*   
</details>


### 🔄 Platform changes!
One of the requirements for getting permission to include **[Nightfall](https://www.curseforge.com/minecraft/mc-mods/epicfight-nightfall)** and **[Gabou's Libs](https://www.curseforge.com/minecraft/mc-mods/gabous-libs)** was that we publish on CurseForge. Combined with a few technical reasons, we have decided to switch to CurseForge **permanently**!   
*(Project on Modrinth has been deleted and **`v0.1.0-alpha-r.dev`-`v0.1.9-alpha-r.dev`** is no longer available for the public).*



***Please note: we do not condone in republishing this modpack without the permission from the author of this modpack anymore.***    
*(Please see updated **[license](https://github.com/ImFloofo7/thelastcircuit/blob/Latest/LICENSE.md))***

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
      
  ***The following mods are what one would call "core mods", adding key elements to the gameplay.***    

  *   **[Advanced Finders](https://www.curseforge.com/minecraft/mc-mods/advanced-finders)** - *Adds specialized ore detection tools* 
  *   **[Advanced Hook Launchers](https://www.curseforge.com/minecraft/mc-mods/advanced-hook-launchers)** - *Adds 3 specialized hooks with distinct mechanics.*   
  *   **[Distant Friends](https://www.curseforge.com/minecraft/mc-mods/distant-friends)** - *Adds stalking player-like mobs that creep at you from a distance.*   
  *   **[Epic Fight - Bosses'Rise](https://www.curseforge.com/minecraft/mc-mods/bossesrise)** - *Adds souls-like bosses, dungeons and loot.*     
  *   **[Fight Back](https://www.curseforge.com/minecraft/mc-mods/fight-back)** - *Adds powerful tools and armor to defend yourself against the dark entities that haunt your world.*   
  *   **[HIM - Herobrine](https://www.curseforge.com/minecraft/mc-mods/him-herobrine)** - *Stalking entity*     
  *   **[Immersive Engineering](https://www.curseforge.com/minecraft/mc-mods/immersive-engineering)** - *Adds lots of realism-inspired technology*     
  *   **[Laser IO](https://www.curseforge.com/minecraft/mc-mods/laserio)** - *EnderIO Pipes but reworked, and with additional content.*     
  *   **[LittleTiles](https://www.curseforge.com/minecraft/mc-mods/littletiles)** - *Adds the ability to create micro (pixel) blocks.*     
  *   **[MagiTech: Arcane Engineering](https://www.curseforge.com/minecraft/mc-mods/magitech-arcane-engineering)** - *Adds "MagiTech", combinging magical and engineering elements with a progression tree centered around minerals.* 
  *   **[Pack-a-Punch Machine](https://www.curseforge.com/minecraft/mc-mods/pack-a-punch-machine)** - *Adds the option to upgrade weapons. Full support for **Tacz** and vanilla firearms.*     
  *   **[Sanity: Renewed](https://www.curseforge.com/minecraft/mc-mods/sanity-renewed)** - *Introduces a sanity meter inspired by Don't Starve, adding a new mechanic that forces players to manage their mental state alongside hunger and health.*     
  *   **[TacZ: AoS](https://www.curseforge.com/minecraft/mc-mods/tacz-art-of-sniping)** - *Lets you snipe entities from extreme distances with realistic ballistics.*     
  *   **[TacZ Attributes](https://www.curseforge.com/minecraft/mc-mods/tacz-attributes)** - *Adds more than 250 attributes to TacZ weapons*     
  *   **[The Final Goatman](https://www.curseforge.com/minecraft/mc-mods/the-final-goatman)** - *Adds a terrifying cryptid*      
  *   **[Underground Villages, Stoneholm](https://www.curseforge.com/minecraft/mc-mods/underground-villages-stoneholm)** - *Adds new villages underground*     
  *   **[Vulcan's Flashlights](https://www.curseforge.com/minecraft/mc-mods/vulcans-flashlights)** - *Adds flashlights, miner's helmets and more.*     
  *   **[Wan's Bio-Scanner](https://www.curseforge.com/minecraft/mc-mods/wans-bio-scanner)** - *Faction tracking and specialized entity identification.*   
  *   **[Wayfinder](https://www.curseforge.com/minecraft/mc-mods/wayfinder)** - *Adds a friendly mob that helps you find biomes*   
  *   **[When Dungeons Arise](https://www.curseforge.com/minecraft/mc-mods/when-dungeons-arise)** - *Adds massive dungeons to your world*   
  *   **** - **   
   </details>

   <details>
    <summary>QoL & Other</summary>

***Mods that tweaks the world, particles, mobs, blocks features etc. or adds something that isn't really content***    

  *   **[2032 (world height)](https://www.curseforge.com/minecraft/mc-mods/world-height-2032)** - *Sets the world height limit to Y=2032*   
  *   **[AAA World](https://www.curseforge.com/minecraft/mc-mods/aaa-particles-world)** - *Adds back the lightning effect in older version of **AAA Particles** mod, and more!*   
  *   **[AE2 Tangible Bookmarks](https://www.curseforge.com/minecraft/mc-mods/ae2-tangible-bookmarks)** - *Let's you bookmark items in **AE2** and more!*   
  *   **[AE2 Terminal Scroll Wheel Cycle](https://www.curseforge.com/minecraft/mc-mods/ae2-terminal-cycling)** - *Allows you to use your scroll wheel in various** AE2** terminals*   
  *   **[Auto Swap](https://www.curseforge.com/minecraft/mc-mods/auto-swap)** - *Automates inventory management and equipment swapping*   
  *   **[BetterEnd Cities](https://www.curseforge.com/minecraft/mc-mods/better-end-cities-better-end)** - *Changes to end city generation and loot.*   
  *   **[Draconic Insight](https://www.curseforge.com/minecraft/mc-mods/draconic-insight)** - *Adds an informational "companion" for **Draconic Evolution***   
  *   **[Dough Slime Ball Recipe](https://www.curseforge.com/minecraft/mc-mods/dough-slime-ball-recipe)** - *Create slime with dough from **Farmers Delight** and dye!*   
  *   **[Essential Mod](https://www.curseforge.com/minecraft/mc-mods/essential-mod)** - *Adds lots of enhancements and possibilities like the ability to host multiplayer worlds for free!*     
  *   **[FastFind](https://www.curseforge.com/minecraft/mc-mods/fastfind)** - *Helps you locate specific items inside any inventory block — `chests`, `furnaces`, `hoppers`, `shulker boxes`, `barrels`, you name it.*   
  *   **[First-person Model](https://www.curseforge.com/minecraft/mc-mods/first-person-model)** - *Client-side mod that changes what you see in 1st person*   
  *   **[Fog](https://www.curseforge.com/minecraft/mc-mods/fog)** - *A total overhaul of Minecraft's fog, offering many different options for customization.*   
  *   **[Inventory HUD+](https://www.curseforge.com/minecraft/mc-mods/inventory-hud-forge)** - *Overhauled Inventory with lots of options and customizeability.*   
  *   **[Inventory Mending](https://www.curseforge.com/minecraft/mc-mods/inventory-mending)** - *Takes away the need to hold the tools with mending*   
  *   **[KubeJS Apothic](https://www.curseforge.com/minecraft/mc-mods/apothic-xp-fix)** - *Fixes/changes how experience costs from Apothic Enchanting are handled.*   
  *   **[Keep Inventory Always](https://www.curseforge.com/minecraft/mc-mods/keep-inventory-always)** - *Turns on the `KeepInventory` gamerule by default.*   
  *   **[Not Enough Animations](https://www.curseforge.com/minecraft/mc-mods/not-enough-animations)** - *Adds/modifies a lot of missing third-person animations from first-person*    
  *   **[PatPat](https://www.curseforge.com/minecraft/mc-mods/patpat)** - *Let's you pat mobs!*    
  *   **[Punchy!](https://www.curseforge.com/minecraft/mc-mods/punchy)** - *Engine for various first-person animations.*    
  *   **[Refined Storage Warning](https://www.curseforge.com/minecraft/mc-mods/rs-storage-warnings)** - *Warns you when **Refined Storage** storage capacity is low *   
  *   **[Resourcify](https://www.curseforge.com/minecraft/mc-mods/resourcify)** - *In-game resource pack, data pack and shader browser + updater.*   
  ((  *   **[Roxy](https://www.curseforge.com/minecraft/mc-mods/roxy)** - *Allows **Voxy** (that is for fabric) to work on NeoForge*   ))     
  *   **[Search for Iris Shaders](https://www.curseforge.com/minecraft/mc-mods/searchfor)** - *Native integration for directory navigation inside shader options.*   
  *   **[SeeU](https://www.curseforge.com/minecraft/mc-mods/seeu)** - *Makes distant players visible far beyond vanilla entity tracking, Compatible with **Voxy***   
  *   **[Spawn Animations](https://www.curseforge.com/minecraft/mc-mods/spawn-animations-mod)** - *Adds fancy spawn animations to mobs!*     
  *   **[Stack Refill](https://www.curseforge.com/minecraft/mc-mods/stack-refill)** - *Automatically replaces exhausted resources from backpack reserves.*   
  *   **[Streams Reflowing](https://www.curseforge.com/minecraft/mc-mods/streams-reflowing)** - *Creates beautiful weaves and wonderful waterways in your world.*   
  *   **[Thunderhead](https://www.curseforge.com/minecraft/mc-mods/thunderhead)** - *Lightning & Thunder overhaul.*   
  *   **[Visual Workbench](https://www.curseforge.com/minecraft/mc-mods/visual-workbench)** - *Items remain physically dropped inside the crafting grid matrix.*   
  *   **[Vulcan's Darkness](https://www.curseforge.com/minecraft/mc-mods/vulcans-darkness)** - *Adds darkness to the world*   
  *   **** - **   
    </details>


    
   <details>
    <summary>Optimization</summary>
   
***The following mods has been added to improve quality and performance***   

  *   **[All The Leaks](https://www.curseforge.com/minecraft/mc-mods/alltheleaks)** - *Crash prevention and optimization*   
  *   **[Create: Better FPS](https://www.curseforge.com/minecraft/mc-mods/create-better-fps)** - *Greatly improves your fps when using Shaderpacks with **Create** mods.*   
  *   **[Entity Culling](https://www.curseforge.com/minecraft/mc-mods/entityculling)** - *Mod that enables the option to skip rendering things that are not in you FoV*     
  *   **[Epic Fight (FPS Optimizer)](https://www.curseforge.com/minecraft/mc-mods/epic-fight-fps-optimizer)** - *A configurable client-side FPS optimizer, reduces distant animation and visual effect rendering costs*   
  *   **[Fast Noise](https://www.curseforge.com/minecraft/mc-mods/zfastnoise)** - *Modern optimization mod to improve world generation times.*     
  *   **[Just Enough Threads](https://www.curseforge.com/minecraft/mc-mods/just-enough-threads)** - *Optimizes **JEI** startup by moving the heaviest startup work off the main thread and spreads it across your CPU cores.*   
  *   **[Not Enough Crashes](https://www.curseforge.com/minecraft/mc-mods/not-enough-crashes-forge)** - *Instead of having to reload the whole pack etc, you get booted back to the main menu when you crash **usually atleast, there are some bugs with this and some irrecoverable crashes that will still crash your whole game.***     
  *   **[PackForge](https://www.curseforge.com/minecraft/mc-mods/packforge-optimized-resource-pack-loading-time)** - *Mod that helps large resource packs load faster.*   
  *   **[Quick Pack](https://www.curseforge.com/minecraft/mc-mods/quick-pack)** - *Improves datapack & resourcepack zip gile loading times.*     
  *   **[Saturn](https://www.curseforge.com/minecraft/mc-mods/saturn)** - *Optimized memory usage and re-mapped memory leak garbage tracking.*   
  *   **[Smooth Boot (Recreated)](https://www.curseforge.com/minecraft/mc-mods/smooth-boot-recreated)** - *Smooth loading allocations across split core processing.*   
  *   **[TacZ: Gunpack Redistribution](https://www.curseforge.com/minecraft/mc-mods/tacz-gunpack-redistribution-fork)** - *Small compatibility utility for **TacZ**.*   
  *   **[TT20](https://curseforge.com)** - *TT20 helps reduce lag by optimizing how ticks work when the server's TPS is low.*   
  *   **** - **   
   </details>

   <details>
    <summary>Add-ons</summary>    
 
***The following mods are add-ons for mods already in the modpack.***   

  *   **[Applied Delight](https://www.curseforge.com/minecraft/mc-mods/applied-delight)** - *Adds a Wireless Cooking Pot, a **Farmer's Delight** pot that pulls ingredients from **AE2** networks*   
  *   **[BetterF3 Spark Module](https://www.curseforge.com/minecraft/mc-mods/betterf3-spark-module)** - *Add-on for **BetterF3** that directly links hardware monitoring with the F3 menu interface.*       
  *   **[Farmer's Cutting: Regions Unexplored](https://www.curseforge.com/minecraft/mc-mods/farmers-cutting-regions-unexplored)** - *Adds more **Farmer's Delight** cutting board recipes for **Regions Unexplored**.*   
  *   **[(IU) Power Utilities](https://www.curseforge.com/minecraft/mc-mods/power-utilities-iu)** - *Add-on to **Industrial Upgrade**. Adds a block that allows you to convert energy from one type to another, and then back.*   
  *   **[(IU) Simply Quarries](https://www.curseforge.com/minecraft/mc-mods/simply-quarries)** - *Add-on for **Industrial Upgrade** that adds a quarry block.*   
  *   **[(IU) Watering Can](https://www.curseforge.com/minecraft/mc-mods/iu-watering-can)** - *Adds watering cans to** Industrial Upgrade**.*   
  *   **[Just Enough Items: AE2](https://www.curseforge.com/minecraft/mc-mods/ae2-jei-integration)** - *Reintroduces the **Just Enough Items** compatibility layer that **Applied Energetics 2** removed in 1.21*   
  *   **[Just enough Items: Create Compat](https://www.curseforge.com/minecraft/mc-mods/createjeicompat)** - *A compatibility mod for **Create** and JEI that enhances the display of sequenced assembly recipes in **JEI** for 7+ steps.*      *   **[Just Enough Items: Effect Descriptions](https://www.curseforge.com/minecraft/mc-mods/just-enough-effect-descriptions-jeed)** - *Provides useful information regarding status effects.*    
  *   **[Just Enough Items: Enchants](https://www.curseforge.com/minecraft/mc-mods/jei-enchants)** - *Adds enchantment-related information to **JEI**.*     
  *   **[Just Enough Items: Filters](https://www.curseforge.com/minecraft/mc-mods/just-enough-filters)** - *Adds a dedicated filter bar to your item list*   
  *   **[Just Enough Items: Malum](https://www.curseforge.com/minecraft/mc-mods/jei-malum)** - *Add-on for **Malum**, designed to display spirit and soul harvesting drop information in JEI.*   
  *   **[Just Enough Items: Mekanism Generatiors](https://www.curseforge.com/minecraft/mc-mods/mekagenjei-mekanism-generator-addon)** - *Adds new custom JEI categories based on **Mekanism Generators***  
  *   **[Just Enough Items: Mekanism Multiblocks](https://www.curseforge.com/minecraft/mc-mods/just-enough-mekanism-multiblocks)** - *Adds a JEI page about **Mekanism** mod's multiblocks.*       
  *   **[Just Enough Items: Refined Storage](https://www.curseforge.com/minecraft/mc-mods/refined-storage-jei-integration)** - *Enhances crafting and recipe interaction between **JEI** and **Refined Storage**.*     
  *   **[Just Enough Items: Resorces](https://www.curseforge.com/minecraft/mc-mods/just-enough-resources-jer)** - *Adds info about mob drops, dungeon loot, ore gen and plant drops*     
  *   **[Just Enough Items: Search](https://www.curseforge.com/minecraft/mc-mods/just-enough-search-jes)** - *Add-on that improves the search experience with better clearing, autocomplete suggestions, search history and favorites.*   
  *   **[Just Enough Items: Sophisticated Backpacks](https://www.curseforge.com/minecraft/mc-mods/sophisticated-jei-index)** - *Adds a JEI Index Upgrade for **Sophisticated Backpacks**.*  
  *   **[Just Enough Items: Structures](https://www.curseforge.com/minecraft/mc-mods/jei-structures)** - *Adds structure information browsing to **JEI**.*  
  *   **[Just Enough Items: WorldGen](https://www.curseforge.com/minecraft/mc-mods/jei-worldgen)** - *View ore generation information from inside JEI (compatible with the majority of modded ores since it reads directly from the biome data).*     
  *   **[Just Enough TacZ](https://www.curseforge.com/minecraft/mc-mods/jet-just-enough-tacz)** - *This mods adds config that allows removal of guns and addons from the game*     
  *   **[Loot Integrations: Yung Structures](https://www.curseforge.com/minecraft/mc-mods/yung-structures-addon-for-loot-integrations)** - *Addon for **Loot Integrations**, changes loot-table for the Yung mod's structures:*    
  *   **[Loot Integrations: Randomized Loot](https://www.curseforge.com/minecraft/mc-mods/vanilla-loot-addon-for-loot-integrations)** - *Addon for Loot Integrations that enhances loot variety in standard chest loot tables.*    
  *   **[ME Requester](https://www.curseforge.com/minecraft/mc-mods/merequester)** - *Easy automation methos to keep **AE2** ME-system "in stock"*   
  *   **[Mekanism Turrets & Fences](https://www.curseforge.com/minecraft/mc-mods/mekanism-turrets-fences)** - *Adds defensive turrents and fences*     
  *   **[Mekanism Jade Upgrades](https://www.curseforge.com/minecraft/mc-mods/mekajadeupgrades)** - *Addon that adds extra tooltips on **Jade** to show installed upgrades in **Mekanism** machines*   
  *   **[Refinded Storage: Delight](https://www.curseforge.com/minecraft/mc-mods/refined-delight)** - *Adds a Wireless Cooking Pot, a **Farmer's Delight** pot that pulls ingredients from **Refined Storage** networks*   
  *   **[Refined Storage: Extra Disks](https://www.curseforge.com/minecraft/mc-mods/extra-disks)** - *Adds bigger fluid- and item disks to **Refined Storage***     
  *   **[Refinded Storage: Fluid Substitution](https://www.curseforge.com/minecraft/mc-mods/refined-fluid-substitution)** - *Allows fluids to be used directly instead of buckets to **Refined Storage***   
  *   **[Refined Storage: Types](https://www.curseforge.com/minecraft/mc-mods/refined-types)** - *Adds support for FE Source and Souls in various **Refined Storage** components*   
  *   **[Sophisticated Tactical Backpacks](https://www.curseforge.com/minecraft/mc-mods/sophisticated-tactical-backpacks)** - *Add-on for **Sophisticated Backpacks** that adds military-style camouflage appearance and an Ammo Reload Upgrade that is compatible with several firearm mods (like **TacZ**).*    
  *   **[TacZ Addon](https://www.curseforge.com/minecraft/mc-mods/tacz-addon)** - *An expansion mod for **TaCZ**.*   
  *   **[TacZ Attributes (Addon)](https://www.curseforge.com/minecraft/mc-mods/tacz-attributes-addon)** - *Transform every gun into a unique find.*   
  *   **[TacZ: Blueprints Reforged](https://www.curseforge.com/minecraft/mc-mods/tacz-blueprints-reforged)** - *Add-on for TaCZ that turns guns and attachments into something you have to discover and earn.*   
  *   **[TacZ Veil Lights](https://www.curseforge.com/minecraft/mc-mods/veil-lights-for-tacz)** - *Add-on that renders configured **TaCZ** weapon lights through the separate **Veil Volume Lights library***   
  *    **** - **   
   </details>


   <details>
    <summary>Integrations & Compatibility</summary>    

***The following mods has been added to add suport and compability between mods.***   

  *   **[Ars Mekanica](https://www.curseforge.com/minecraft/mc-mods/ars-mekanica)** - *A compatibility addon that bridges **Ars Nouveau** and **Mekanism**.*   
  *   **[BetterEnd x Chipped](https://www.curseforge.com/minecraft/mc-mods/betterend-chipped)** - *Massive expansion of decorative variant choices for end-materials.*   
  *   **[CIT Resewn](https://www.curseforge.com/minecraft/mc-mods/cit-resewn)** - *Re-implements **MCPatcher's CIT***   
  *   **[CITResewnNeoPatcher](https://www.curseforge.com/minecraft/mc-mods/cit-resewn-neopatcher)** - *Patches CIT Resewn mods so it runs on NeoForge through **Sinytra Connector***   
  *   **[Dynamic Trees x BetterNether](https://www.curseforge.com/minecraft/mc-mods/dynamictrees-betternether)** - *Bring **Dynamic Trees** support to the trees and fungi added by **BetterNether**.*   
  *   **[Dynamic Trees x BetterEnd](https://www.curseforge.com/minecraft/mc-mods/dynamictrees-betterend)** - *Bring **Dynamic Trees** support to the trees and giant fungi added by **BetterEnd**.*   
  *   **[EMF Comapt: Carry On](https://www.curseforge.com/minecraft/mc-mods/emf-compat-carry-on)** - *A small client-side mod that makes Carry On carry poses work correctly with Entity Model Features player models.*   
  *   **[EMF Compat: Core](https://www.curseforge.com/minecraft/mc-mods/emf-compat-core)** - *A shared client-side library that lets all EMF Compat addons fix animation conflicts with Entity Model Features.*   
  *   **[EMF Compat: Malum](https://www.curseforge.com/minecraft/mc-mods/emc-for-malum)** - *Adds compatibility between **ProjectE** and **Malum***   
  *   **[EMF Compat: Not Enough Animations](https://www.curseforge.com/minecraft/mc-mods/emf-compat-not-enough-animations)** - ***Entity Model Features: player animations** while **Not Enough Animations** is active.*   
  *   **[EMF Comapt: Physics](https://www.curseforge.com/minecraft/mc-mods/physics-emf-compat)** - *This allows resource packs that use **EMF** — such as **Fresh Animations** — to work correctly with **Physics Mod's** ragdoll and other physics modes.*   
  *   **[EMF Compat: TACZ](https://www.curseforge.com/minecraft/mc-mods/emf-compat-tacz)** - *Adds EMF compatibility for **TacZ***   
  *   **[Epic Fight Auto Compat](https://www.curseforge.com/minecraft/mc-mods/epic-fight-auto-compat)** - *Background translation framework for out-of-the-box combat styles.*   
  *   **[Epic Fight: Curios Compat 2.0](https://curseforge.com)** - *Adds compatibility/fix between **Curios** and **Epic Fight***   
  *   **[Epic Fight: Curios Elytra](https://www.curseforge.com/minecraft/mc-mods/epicurios-elytra-epic-fight-elytra-slot-compat-fix)** - *Allows slotting of standard flight parameters inside Curios accessories.*   
  *   **[Epic Fight x Punchy](https://curseforge.com)** - *Adds compatibility between **Punchy** and **Epic Fight***   
  *   **[Epic Fight: Tweaks](https://www.curseforge.com/minecraft/mc-mods/epic-tweaks)** - *Core adjustments for overall damage parameters and entity behaviors.*   
  *   **[Evolved Mekanism JEI Compat](https://www.curseforge.com/minecraft/mc-mods/evolved-mekanism-jei-emi-compat)** - *Adds compatibility between **Evolved Mekansim** and **JEI***   
  *   **[Iris Veil Compat](https://www.curseforge.com/minecraft/mc-mods/iris-veil-compat)** - *Allow mods using the Veil rendering engine to render correctly when using Iris Shaderpacks.*   
  *   **[Jade Additional Entities](https://www.curseforge.com/minecraft/mc-mods/jade-additional-entities)** - *Adds support for displaying information from **Jade** on entities added by other mods.*   
  *   **[Loot Integrations](https://www.curseforge.com/minecraft/mc-mods/loot-integrations)** - *Implemented global looting balance patches covering ***Born in Chaos**, **L_ender's Cataclysm**, **Integrated**, **Yung's**, and Vanilla variables.*   
  *   **[Loot Integrations: Born in Chaos](https://www.curseforge.com/minecraft/mc-mods/loot-integrations-cataclysm)** - *Enhances loot for **Born in Chaos** structures and bosses.*    
  *   **[Loot Integrations: L_Ender's Cataclysm](https://www.curseforge.com/minecraft/mc-mods/loot-integrations-cataclysm)** - *Enhances loot for **L_Ender's Cataclysm**structures and bosses.*   
  *   **[Macaw's Betters](https://www.curseforge.com/minecraft/mc-mods/macaws-betters)** - *Adds multi-compatibility for **Macaw's**.. 
        * **Bridges**
        * **Doors**
        * **Fences**
        * **Furnitures**
        * **Paths**
        * **Roofs**
        * **Stairs**
        * **Trapdoors**
        * **Windows**
        ** and the mods: **Better Nether** and **Better End**.*   
  *   **[Mystical Agriculture Compats](https://www.curseforge.com/minecraft/mc-mods/mystical-agriculture-compats)** - *Adds compatibility between **Mystical Agriculture**, **Mekanism's** Enrichment Chamber and EnderIO's SAG Mill* 
  *   **[Mystical Engineering](https://www.curseforge.com/minecraft/mc-mods/mystical-engineering)** - *Adds comaptibility between **Mystical Agriculture** and Immersive Engineering's "Garden Clocke"*   
  *   **[ReIntegrated: Chipped](https://www.curseforge.com/minecraft/mc-mods/reintegrated-chipped)** - *Smoothly integrates the blocks from the Chipped mod into vanilla's biomes and structures.*   
  *   **[Spawn Animations Compat](https://www.curseforge.com/minecraft/mc-mods/spawn-animations-compats)** - *Adds compatibility between **Spawn animations** and 50+ mods !*   
  *   **[TacZ: Curios](https://www.curseforge.com/minecraft/mc-mods/taczcurios)** - *TaczCurios adds custom curios (accessories) to the mod **TacZ***   
  *    **** - **   
   </details> 


   <details>
    <summary>Misc</summary>  

***Libraries, engines and more required mods.***   

  *   **[AAA Particles](https://www.curseforge.com/minecraft/mc-mods/aaa-particles)** - *Library mod that enables using effekseer particles (`.efkefc`) in minecraft.*   
  *   **[Advanced Wall Climber API](https://www.curseforge.com/minecraft/mc-mods/advanced-wall-climber-api)** - *API that enables advanced wall climbing mechnaics for entities.*   
  *   **[Animatica "Foxified"](https://www.curseforge.com/minecraft/mc-mods/animatica-foxified)** - *Animatica unofficial NeoForge port that load the **MCPatcher**/**Optifine** animeted texture format.*   
  *   **[Apothic Attributes](https://www.curseforge.com/minecraft/mc-mods/apothic-attributes)** - *library mod that provides a variety of attributes and attribute-related utilities.*    
  *   **[Berezka Library](https://www.curseforge.com/minecraft/mc-mods/berezka-library)** - *Library mod for **Just Enough TacZ***   
  *   **[Better Library](https://www.curseforge.com/minecraft/mc-mods/better-library)** - *Simple library for config*   
  *   **[Configured](https://www.curseforge.com/minecraft/mc-mods/configured)** - *Dynamically creates configuration menus for every mod with a supported config system.*   
  *   **[CodeChicken Lib](https://www.curseforge.com/minecraft/mc-mods/codechicken-lib-1-8)** - *Library mod for "Chicken-Bones" mods*   
  *   **[CreativeCore](https://www.curseforge.com/minecraft/mc-mods/creativecore)** - *Core for **LittleTiles***     
  *   **[Cupboard](https://www.curseforge.com/minecraft/mc-mods/cupboard)** - *Provides code, different frameworks and utilities for minecraft mods*   
  *   **[Deimos Lib](https://www.curseforge.com/minecraft/mc-mods/deimos-fabric-forge-neoforge)** - *A data generation and configuration library*   
  *   **[DragonLib](https://www.curseforge.com/minecraft/mc-mods/dragonlib)** - *Multiloader library and framework built on **Architectury API***     
  *   **[Eating Animation (Core)](https://www.curseforge.com/minecraft/mc-mods/eating-animation-forge)** - *Restores fundamental consumption mechanics for base items.*       
  *   **[Forgified Fabric API](https://www.curseforge.com/minecraft/mc-mods/forgified-fabric-api)** - *Fabric API implemented on top of NeoForge*   
  *   **[ForgeEndertech](https://www.curseforge.com/minecraft/mc-mods/forgeendertech)** - *Core library for **Large Ore Deposits**, **Advanced Hook Launchers** and **Advanced Finders***   
  *   **[FTB Certain Question additions](https://www.curseforge.com/minecraft/mc-mods/certain-questing-additions)** - *Adds a few minor improvements and smooth animations to **FTB Quests** mod.*   
  *   **[FTB Extra Quests](https://www.curseforge.com/minecraft/mc-mods/extraquests)** - *Add-on that adds new tasks, rewards and functions. - **For upcoming changes/features***   
  *   **[FTB ExtraLib](https://www.curseforge.com/minecraft/mc-mods/extralib)** - *Library for **ExtraQuests***   
  *   **[FTB Library](https://www.curseforge.com/minecraft/mc-mods/ftb-library-forge)** - *Library for **FTB Quests**.*   
  *   **[FTB Quests](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-forge)** - *Quest book system*   
  *   **[FTB Quests: Completion Broadcast](https://www.curseforge.com/minecraft/mc-mods/quest-completion-broadcast)** - *Chat announcements for quest, (including for players on other teams).*   
  *   **[FTB Quests: Enhance](https://www.curseforge.com/minecraft/mc-mods/quest-enhance)** - *Client-side "enhancement" mod for **FTB Quests***   
  *   **[FTB Quests: Entity Visualization](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-entity-visualization)** - *This mod replaces the boring spawn‑egg icon in a kill task with the actual entity rendered live in 3D.*   *   **[FTB Quests: Optimizer](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-optimizer)** - *Removes micro-freezes when moving items and turning in quests, makes inventory checking smarter and quieter for the server*     *   **[FTB Quests: Quick Check](https://www.curseforge.com/minecraft/mc-mods/ftb-quest-quick-check)** - *Adds a button to the **FTB Quests** GUI that completes all currently available "checkmark" tasks in one action.*   
  *   **[FTB Teams](https://www.curseforge.com/minecraft/mc-mods/ftb-teams-forge)** - *Library for mods that can utilize team progression like **FTB Chunks** and **FTB Quests**.*   
  *   **[Fzzy Config](https://www.curseforge.com/minecraft/mc-mods/fzzy-config)** - *A powerful configuration engine*     
  *   **[GroovyModLoader (GML)](https://www.curseforge.com/minecraft/mc-mods/gml)** - *Lower-level back end optimization for early mod setup strings.*   
  *   **[Konkrete](https://www.curseforge.com/minecraft/mc-mods/konkrete)** - *Another Library mod*   
  *   **[Kotlin for Forge](https://www.curseforge.com/minecraft/mc-mods/kotlin-for-forge)** - *Adds a Kotlin language loader and provides some optional utilities.*   
  *   **[KotlinLangForge](https://www.curseforge.com/minecraft/mc-mods/kotlinlangforge)** - *Provides a Kotlin language adapter for Forge and Neoforge*   
  *   **[LDLib](https://www.curseforge.com/minecraft/mc-mods/ldlib)** - *library for UI, rendering, synchronization, persistence, and in-game editors.*   
  *   **[MezzConfig](https://www.curseforge.com/minecraft/mc-mods/mezzconfig)** - *Simple configuration library for mods*   
  *   **[MRU](https://www.curseforge.com/minecraft/mc-mods/mru)** - *Library mod*   
  *   **[Particle Core](https://www.curseforge.com/minecraft/mc-mods/particle-core)** - *Optimizes particles.*   
  *   **[PlayerNBT Quests](https://www.curseforge.com/minecraft/mc-mods/playernbt-quests-ftb-quests)** - *Extension mod that provides quest creators with player NBT data detection functionality. *   
  *   **[Progressive Stages](https://www.curseforge.com/minecraft/mc-mods/progressivestages)** - *Minecraft progression system*   
  *   **[Sophisticated Core](https://www.curseforge.com/minecraft/mc-mods/sophisticated-core)** - *Library mod for "sophisticated" mods.*   
  *   **[SuperMartijn642's Core Lib](https://www.curseforge.com/minecraft/mc-mods/supermartijn642s-core-lib)** - *Adds lots of basic implementations for GUIs, blocks, tile entities, and network packets that allow for similar code between Minecraft 1.12-1.20*   
  *   **[Toadlib](https://www.curseforge.com/minecraft/mc-mods/toadlib)** - *Library mod*   
  *   **[UI Quests](https://www.curseforge.com/minecraft/mc-mods/uiquest)** - *Alternate UI for **FTB Quests***   
  *   **[Veil Volume Lights](https://www.curseforge.com/minecraft/mc-mods/veil-volume-lights)** - *Veil add-on library that adds support for colored mediums.*   
  *   **** - **     
   </details> 


   <details>
      <summary>For Upcoming Changes</summary>

***The following mods have been added for enabling work on some future upcoming changes & features.***   

  *   **[KubeJS](https://www.curseforge.com/minecraft/mc-mods/kubejs)** - *Edit recipies, add new custom items, script world events, all in JavaScript! - **For upcoming changes/features***   
  *   **[KubeJS Additions](https://www.curseforge.com/minecraft/mc-mods/kubejs-additions)** - *KubeJS Integration for JEI(/REI) and Jade. - **For upcoming changes/features***   
  *   **[KubeJS Applied](https://www.curseforge.com/minecraft/mc-mods/applied-kubejs-kjs-ae2)** - *KubeJS bridge that adds scriptable AE2 recipes, network monitoring, storage/crafting events, device inspection, and optional ME crafting job automation. - **For upcoming changes/features***   
  *   **[KubeJS Ars Nouveau](https://www.curseforge.com/minecraft/mc-mods/kubejs-ars-nouveau)** - *Allows KubeJS to create Ars Nouveau Recipies - **For upcoming changes/features***   
  *   **[KubeJS Create](https://www.curseforge.com/minecraft/mc-mods/kubejs-create)** - *Create integration for KubeJS - **For upcoming changes/features***   
  *   **[KubeJS Curios](https://www.curseforge.com/minecraft/mc-mods/kubejs-curios)** - *Curios integration for KubeJS. - **For upcoming changes/features***   
  *   **[KubeJS CustomMeteor](https://www.curseforge.com/minecraft/mc-mods/custommeteorjs)** - *AE2 addon for modpack makers. It lets you control meteorite blocks and terrain behavior without editing AE2 itself. - **For upcoming changes/features***   
  *   **[KubeJS Draconic Evolution](https://www.curseforge.com/minecraft/mc-mods/kubejs-draconic-evolution)** - *Integration for Draconic Evolution fusion crafting. - **For upcoming changes/features***   
  *   **[KubeJS Editor](https://www.curseforge.com/minecraft/mc-mods/kjs-editor)** - *In-game visual editor for KubeJS. It allows you to create, modify, and manage recipes and content directly inside Minecraft without writing code. - **For upcoming changes/features***   
  *   **[KubeJS EnderIO](https://www.curseforge.com/minecraft/mc-mods/kubejs-enderio)** - - *Adds KubeJS integration to EnderIO. - **For upcoming changes/features***   
  *   **[KubeJS Gecko](https://www.curseforge.com/minecraft/mc-mods/geckojs)** - *Allows you to create animatable block/item/armor with Geckolib through KubeJS.* - *For upcoming changes/features***   
  *   **[KubeJS GUI](https://www.curseforge.com/minecraft/mc-mods/kubejs-gui)** - *KubeJS GUI template system to make custom recipes. - *Fpr upcoming changes/features***   
  *   **[KubeJS Immersive Engineering](https://www.curseforge.com/minecraft/mc-mods/immersive-engineering-js)** - *KubeJS integration for Immersive Engineering. - **For upcoming changes/features***    
  *   **[KubeJS IU](https://www.curseforge.com/minecraft/mc-mods/kubejs-iu)** - *Adds configuration possibilities to machine processing recipes of Industrial Upgrade (IU). - **For upcoming changes/features***      
  *   **[KubeJS JEI](https://www.curseforge.com/minecraft/mc-mods/kubejs-jei)** - *Supports creating new JEI recipe display entries, hiding specified items, or re-showing items that have been hidden.*   
  *   **[KubeJS LootJS](https://www.curseforge.com/minecraft/mc-mods/lootjs)** - *Integration to modify the loot tables and loot modifiers. - **For upcoming changes/features***   
  *   **[KubeJS Mekanism](https://www.curseforge.com/minecraft/mc-mods/kubejs-mekanism)** - *Mekanism integration for KubeJS. - **For upcoming changes/features***   
  *   **[KubeJS Mekanism Extends](https://www.curseforge.com/minecraft/mc-mods/kubejs-mekanism-extends)** - *Mekanism **Extends** integration for KubeJS. - **For upcoming changes/features***   
  *   **[KubeJS NeoVitae](https://www.curseforge.com/minecraft/mc-mods/kubejs-neovitae)** - *KubeJS addon for NeoVitae that exposes its custom recipe types to server scripts, so pack authors can add, remove, and customize recipes without touching JSON by hand. - **For upcoming changes/features***  
  *   **[KubeJS Keybinds](https://www.curseforge.com/minecraft/mc-mods/kubejs-keybinds)** - *Expands upon KubeJS by allowing you to modify existing KeyBinds and Categories. - **For upcoming changes/features***   
  *   **[KubeJS Occultism](https://www.curseforge.com/minecraft/mc-mods/occultism-kubejs)** - *Occultism KubeJS provides KubeJS integrations for Occultism. - **For upcoming changes/features***   
  *   **[KubeJS PneumaticCraft: Re-pressurized](https://www.curseforge.com/minecraft/mc-mods/kubejs-pneumaticcraft)** - *PneumaticCraft: Repressurized integration for KubeJS. - **For upcoming changes/features***   
  *   **[KubeJS ProjectE](https://www.curseforge.com/minecraft/mc-mods/kubejs-projecte)** - *Lets you set the EMC values of items and the Philosopher's Stone transformations blocks with the ProjectE mod. - **For upcoming changes/features***     
  *   **[KubeJS Tweaks](https://www.curseforge.com/minecraft/mc-mods/kubejs-tweaks)** - *This is an addon for KubeJS to abstract some common usage of KubeJS for heavly modded modpacks. - **For working on upcoming features***   
  *   **[KubeJS Quest(JS)](https://www.curseforge.com/minecraft/mc-mods/questjs)** - *Adds client-side KubeJS events for the FTB Quests GUI. - **For working on upcoming features***   
  *   **[KubeJS Rechisled](https://www.curseforge.com/minecraft/mc-mods/kubejs-rechiseled)** - *KubeJS integration for Rechisled. - **For upcoming changes/features***   
  *   **** - **   
   </details>
</details>

---

## 🔄Mod Updates & Removals   

<details>
  <summary>Updated</summary>

***The following mods have been updated.***   
  
  *   **CITResewnPatcher** -> Updated from Fabric version *(ran with Sinytra Connector)* to [NeoForge version](https://www.curseforge.com/minecraft/mc-mods/cit-resewn-neopatcher)   
  *   **[AE2 Growth Accelerator Tiers](https://www.curseforge.com/minecraft/mc-mods/ae2-growth-accelerators)** -> Updated from Fabric version *(ran with Sinytra Connector)* to `AGA Neo 1.21.1 2.2.0`   
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
  *   **Zero CORE 2** -> Updated from Zero CORE (1) `2.4.9` to `2.4.21`   
</details>

<details>
  <summary>Removed</summary>  
  
  *Due to incompatibilities, change of vision and more, we've decided to remove the following mods from this version:*   
  *   **[Distant Horizons](https://www.curseforge.com/minecraft/mc-mods/distant-horizons):** *Replaced by Voxy*   
  *   **Every Compat - "[Wood Good](https://www.curseforge.com/minecraft/mc-mods/every-compat)", "[Stone Zone](https://www.curseforge.com/minecraft/mc-mods/stone-zone)", "[Gems Realm](https://www.curseforge.com/minecraft/mc-mods/gems-realm)":** *Removed for now because incompatibility, and other mods like **Almost Unified** cover most of this anyway.*   
  *   **[Create Blocks & Bogies](https://www.curseforge.com/minecraft/mc-mods/create-blocks-bogies):** *Extracted to preserve clean schematic layouts in custom factory builds.*   
  *   **Mekanism: Elements:** *Purged from the environment chain to prevent recipe conflicts with advanced alloy automation.*   

  *   **AE2 Lightning Tech:** *Outdated version and it's "a bit too much"*   
  *   **AE2: Better Villagers:** *Causing fatal `MenuType` error*   
  *   **Create: Better Villagers:** *Causing fatal `MenuType` error*   
  *   **Create Unlimited:** *Unnecessary..*   
  *   **[Create: Gunsmithing:](https://www.curseforge.com/minecraft/mc-mods/cgs)** *It's enough with TacZ.. for now.*   
  *   **[Create: Central Kitchen](https://www.curseforge.com/minecraft/mc-mods/create-central-kitchen)** - *Removed to decrease clutter since there are already lots of kitchen/food releated stuff,*   
  *   **[Create: Bits 'n' Bobs](https://www.curseforge.com/minecraft/mc-mods/create-bits-n-bobs)** - *Removed to decrease clutter.*   
  *   **[Create: Misc & Things](https://www.curseforge.com/minecraft/mc-mods/create-misc-and-things)** - *Removed to decreace clutter.*   

  *   **[Create Threaded Trains](https://www.curseforge.com/minecraft/mc-mods/create-threaded-trains)** - *Addon that is no longer needed due to the removal of **Create Trains***   
  *   **[Create; Track Map: Fork](https://www.curseforge.com/minecraft/mc-mods/create-track-map-fork2)** - *Addon that is no longer needed due to the removal of **Create Trains***   
  *   **[Create; Train Utilities](https://www.curseforge.com/minecraft/mc-mods/create-trainutilities)** - *Addon that is no longer needed due to the removal of **Create Trains***   
  *   **[Create: Train Lights](https://www.curseforge.com/minecraft/mc-mods/create-train-lights)** - *Addon that is no longer needed due to the removal of **Create Trains***   

  *   **[Xaero Train Map](https://www.curseforge.com/minecraft/mc-mods/xaero-train-map)** - *Addon that is no longer needed due to the removal of **Create Trains***   
  *   **** - *Addon that is no longer needed due to the removal of **Create Trains***   
  *   **** - *Addon that is no longer needed due to the removal of **Create Trains***   
  *   **** - *Addon that is no longer needed due to the removal of **Create Trains***   
    *   **[Woodwalkers](https://www.curseforge.com/minecraft/mc-mods/woodwalkers)** - *Removed because redundancy*   
  *   **[Remove Loading Screen:](https://www.curseforge.com/minecraft/mc-mods/rrls)** The mod **Remove loading screen** has been permanently removed from the pack *(removed in v0.1.3-alpha-r.dev)*, as it is **completely** incompatible with our   

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
   *   **** - ** version*   
   *Discover mysterious monoliths and uncover the ancient powers hidden within!*   

---

## Configurations and Custom content:
### Changes   

We're going to start focusing a bit more on various custom changes using 
  * KubeJS 
  * Pachouli
  * FTB Quests
  * Progressive Stages
and other various "integrations", configs etc etc. 

Regarding overall quality, we're also working on mod balancing, quests and atmospheric changes as well as some other improvements, so not just adding more mods and configs.   
Like the FancyMenu changes I mentioned [here](https://github.com/ImFloofo7/thelastcircuit/blob/v0.2.0/Changelog%20v0.2.0-alpha.md#mod-updates--removals:~:text=error-,Remove,menus), to keep the "creepy" horror-like feeling relevant throughout the whole pack *(including menu's and stuff)-*   
For balancing, we will also be making it "*harder*" to gain access to certain items, like powerful guns and spells, implementing a **"immersive" progression system** to balance the modpack and actually make you work to stay alive, using [FTB Quests](https://www.curseforge.com/minecraft/mc-mods/ftb-quests-forge) and [Progression Stages](https://www.curseforge.com/minecraft/mc-mods/progressivestages), amongst others.    


### If you want more sneak peeks, I highly recommend you to..
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












