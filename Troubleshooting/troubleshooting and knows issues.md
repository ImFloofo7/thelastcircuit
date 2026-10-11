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
   
You can if you want, just copy this and put it there, packs that you don't have installed won't be loaded and after a restart remove the strings that are not available.

### Step 5

Press `Ctrl` + `S` to save the changes or in the top left "`File`" > "`Save`" and close the window.

Now you're all done!
Just boot up your instance and enjoy!

</details>