# The Last Circuit v0.2.0 pre-release hotfix

This hotfix focuses on resolving several critical crashes and compatibility issues encountered when accessing **Singleplayer** and preparing new worlds.

---

### 🛠️ Fixes & Changes

- **KubeJS Tweaks** — Updated from `1.0.6` to `1.0.7` to address a critical Mixin injection failure during world creation.
- **Delightful Creators** — Removed due to compatibility issues involving Create's Sequenced Assembly recipe processing.
- **Runelic** — Reset its configuration to address a JSON deserialization error during datapack loading.

---

## ⚠️ Known Issues & Important Notes

### ⏳ World Creation — Extended Loading Times

**World creation can take a considerable amount of time**, especially during **"Preparing for world creation…"**.

*I'm aware of the extended loading times and will continue looking into possible optimizations in future updates.*

- Minecraft may temporarily freeze or display **"Not Responding"** while loading datapacks, recipes, and other resources.
- **This does not necessarily mean the game has crashed.**
- **Please be patient and let the game continue running.** Even if it appears frozen, loading may still complete successfully.

### 📦 CurseForge Installation — The Broken Script / void.jar

> **⚠️ Installation issue under investigation**  
> CurseForge may fail when trying to download the unavailable `project-1240986` as a dependency of **void.jar**. Making `void.jar` optional in Pre-release #2 is an unconfirmed workaround. Read the installation guide below before launching Minecraft.

---

## 🔍 Technical Details & Crash Fixes

For those interested in the technical details, the exact errors encountered during troubleshooting are listed [here](https://github.com/ImFloofo7/thelastcircuit/blob/Latest/All%20Changelogs/v0.2.0-alpha/v0.2.0%20pre-release%20hotfix%20%231.md#-technical-details--crash-fixes).

---

## 📌 Additional Information

Further performance optimizations, stability improvements, and compatibility fixes are planned for future updates.

If you encounter additional issues, please report them through the [official Discord](https://discord.gg/A3TFF6TqEU) or [GitHub Issues](https://github.com/ImFloofo7/thelastcircuit/issues).

**Thank you for your patience and support!** 💙💜

Full changelog can be found [here](https://www.curseforge.com/minecraft/modpacks/the-last-circuit/files/9367250).

---

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
