# 🛠️ Changelog: v0.1.1-alpha

This is a minor update focusing on initial background cleanup, mod management, and loader stability. Please note that while this build is slightly more optimized than **v0.1.0-alpha**, the modpack is still **far from finished**, and you will encounter bugs and unfinished progression lines. 

---

### ⚙️ Optimizations & Fixes
* **Registry Fixes:** Resolved critical NeoForge container crashes (`Adding duplicate value... to registry` on `InitMenuTypes.registerAll`).
* **Background Cleanup:** Removed several conflicting Refined Storage and AE2 add-ons that were locking up the loader's memory.
* **Core Tweaks:** Fine-tuned background caching properties via ModernFix for smoother client boot times.

### 🔄 Mod Updates & Removals
* **Mod Updates:** Several core tech and magic mods have been updated to their latest stable 1.21.1 versions to prevent backend memory leaks.
* **Mod Removals:** Cleared out multiple broken combat/visual compatibilities and duplicate libraries to sanitize the instance.
* **Remove Loading Screen (Removed):** The mod `Remove loading screen` has been permanently removed from the pack, as it is completely incompatible with our upcoming **FancyMenu** UI setup.

---

### ⚠️ IMPORTANT DISCLAIMER (Please Read)
Please make sure to read the full **Disclaimer** section on our official **Modrinth** or **GitHub** pages before playing. 

As a reminder: **Nightfall** and **Gaboulibs** are **NOT** included in this build for the time being. I am currently waiting on official licensing/permissions from the authors before these mods can be safely and legally packaged into the instance. 
