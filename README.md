# Villager Choir 🎶

**Villagers spontaneously form choirs and sing songs together!**

Villager Choir brings your villages to life: nearby villagers gather in a circle, form a choir, and sing together — either on their own (randomly) or on demand via commands or the in-game GUI. You can even add your own custom songs!

---

## ✨ Features

-  **Spontaneous performances** – Villagers can start singing on their own based on configurable chance and cooldown.
-  **Circle formation** – Choir members walk into a circle around the singer before the song begins.
-  **In-game GUI** – Open the control screen to start/stop performances and tweak settings live.
-  **Commands** – Full command control with `/villagerchoir` (see below).
-  **Custom songs** – Drop your own `.ogg` files into the custom songs folder and they become available songs.
-  **Client-side config sync** – Settings from the GUI are synced to the server session.
-  **Debug mode** – Optional debug logging and a debug circle visualization to tune formation.

---

## 📦 Supported Versions

| Minecraft | Loader |
|-----------|--------|
| 1.21.1 | Fabric, Forge, NeoForge |
| 1.21.2 | Fabric, NeoForge |
| 1.21.3 | Fabric, NeoForge |
| 1.21.4 | Fabric, NeoForge |
| 1.21.5 | Fabric, NeoForge |
| 1.21.6 | Fabric |
| 1.21.7 | Fabric, NeoForge |
| 1.21.8 | Fabric, NeoForge |
| 26.1.2 | Fabric |

> **Note:** In 1.21.x, Forge and NeoForge split into separate mod loaders — make sure you download the correct build for your loader.

---

## 🔧 Recommended Settings

> ⚠️ **Recommended:** Set the **GUI Scale** in Minecraft's video settings to **2x** for the best experience with the Villager Choir screen.

You can change this in-game via **Options → Video Settings → GUI Scale** (set to `2`).

---

## 📥 Installation

1. Install the mod loader for your Minecraft version ([Fabric](https://fabricmc.net/use/) / [Forge](https://files.minecraftforge.net/) / [NeoForge](https://neoforged.net/)).
   - Fabric also requires [Fabric API](https://modrinth.com/mod/fabric-api).
2. Download the correct JAR from the [`fabric/`](fabric/), [`forge/`](forge/), or [`neo/`](neo/) folder of this repository.
3. Place it in your `.minecraft/mods` folder.
4. Launch the game!

**Requirements:**
- **Java 21+** (Minecraft 1.21+ requirement)
- **Fabric Loader 0.16+** (Fabric builds)

---

## 🎮 Usage

### In-game GUI

Press the **Villager Choir** keybind (configurable in *Options → Controls → Key Binds*) to open the control screen. From there you can:

- Start/stop a performance
- Pick the song, formation, and circle radius
- Tune join radius, max participants, singing chance, and cooldown
- Toggle random singing and debug logging

### Commands

```
/villagerchoir start            # Start a performance near you
/villagerchoir stop             # Stop the active performance
/villagerchoir debug            # Toggle debug logging / debug circle
/villagerchoir reload           # Reload custom songs from the songs folder
```

---

## 🎵 Adding Custom Songs

1. Go to your `.minecraft` folder and find the Villager Choir custom songs directory (auto-created on first run).
2. Drop your `.ogg` files inside (pack format 34 for resource-pack style song folders).
3. Run `/villagerchoir reload` in-game (or use the GUI).
4. Your songs now appear in the song list!

---

## 🛠️ Configuration

Settings are stored in `villagerchoir.json` in your config folder. Most options can also be changed live from the in-game GUI.

| Setting | Description |
|---------|-------------|
| Chance | How likely villagers are to spontaneously start singing |
| Cooldown | Time between spontaneous performances |
| Join Radius | How far villagers will travel to join the choir |
| Max Choir | Maximum number of singers in a choir |
| Circle Radius | Radius of the circle formation |
| Formation | Circle formation type (incl. circle walk) |
| Random Singing | Enable/disable spontaneous performances |
| Chat Log / Debug Logging | Verbose logging for troubleshooting |

---

## 📄 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT) — Copyright (c) 2024 VillagerChoir.

---

*Made with ❤️ for Minecraft village lovers. Enjoy the choir! 🎶*
