<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/0a0afad5-241f-4079-865d-c33ef0d04d32" />

# Loading Screen

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

If this doesn't fix the issue, please open a ticket in the [discord](https://discord.gg/CkaUdd5YDk) or submit an issue here on GitHub.
