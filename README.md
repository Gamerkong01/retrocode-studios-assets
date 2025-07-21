# retrocode-studios-assets
Official asset library for RetroCode Studios.
# 🎮 RetroCode Studios Asset Library 🎨

This repository serves as the official asset library for **RetroCode Studios**, providing a curated collection of game-ready assets across various genres, optimized for use in your web-based retro game projects.

---

## Table of Contents
- [About This Library](#about-this-library)
- [Asset Categories](#asset-categories)
- [How to Use These Assets in RetroCode Studios](#how-to-use-these-assets-in-retrocode-studios)
- [Licensing](#licensing)
- [Contributing](#contributing)
- [Support & Community](#support--community)

---

## About This Library

We believe in making retro game development accessible and fun. RetroCode Studios is an online platform that empowers creators to build browser-based retro games without needing complex software installations.

**Important Note:** The assets provided in this library are sourced exclusively from [Kenney.nl](https://kenney.nl/), a fantastic resource for game developers. **RetroCode Studios did NOT create these assets.** We are simply providing a curated, convenient collection for use within our platform, all under the generous licensing provided by Kenney.

---

## Asset Categories

Our assets are organized into clear categories and thematic packs to help you find what you need quickly. Click on a category name to browse the assets directly on GitHub.

### 🚀 Shooter Assets
[Explore Shooter Assets]([https://github.com/Gamerkong01/retrocode-studios-assets/tree/main/SHOOTER](https://github.com/Gamerkong01/retrocode-studios-assets/tree/c4ec4088c69813391f36bcef04717474d8619f33/Top%20Down%20Shooter))
* **Space Shooter Redux:** Classic top-down space assets from Kenney.nl, including ships, lasers, and backgrounds.
* **Top-Down Shooter Pack:** Spritesheets and individual sprites suitable for various top-down shooter styles.

### 🏰 RPG Assets
[Explore RPG Assets](https://github.com/Gamerkong01/retrocode-studios-assets/tree/main/RPG)](https://github.com/Gamerkong01/retrocode-studios-assets/tree/c4ec4088c69813391f36bcef04717474d8619f33/RPG)
* **Fantasy RPG Pack 1:** Characters, tilesets, and sounds for a fantasy adventure, perfect for pixel-art RPGs.
* **Sci-Fi RPG Pack A:** Sci-fi themed sprites, environmental elements, and UI components for futuristic RPGs.

### 🏃 Platformer Assets
[Explore Platformer Assets][(https://github.com/Gamerkong01/retrocode-studios-assets/tree/c4ec4088c69813391f36bcef04717474d8619f33/Platformer)
* **New Platformer Pack:** Core characters, props, and tiles for fresh platformer experiences.
* **Platformer Pack Redux:** Extended tilesets, backgrounds, and additional characters.
* **Platformer Art Extended Enemies:** A wide variety of enemy sprites to populate your platforming worlds.

### ⚽ Sport Assets
[Explore Sport Assets](https://github.com/Gamerkong01/retrocode-studios-assets/tree/c4ec4088c69813391f36bcef04717474d8619f33/Sports)
* **Retro Soccer Pack:** Pixel-art style assets for a classic retro soccer game, including players and ball sprites.
* **Basketball Court Kit:** Tiles and sprites for building detailed basketball court environments.

---

## How to Use These Assets in RetroCode Studios

To seamlessly integrate any asset from this library into your RetroCode Studios project (which leverages Phaser.js/Pixi.js for game development), you'll need the direct **raw GitHub URL** for each specific file.

**Quick Steps:**
1.  On this GitHub repository, navigate to the desired asset file (e.g., `SHOOTER/SpaceShooterRedux/PNG/playerShip1_blue.png`).
2.  Click the **"Raw"** button (usually at the top right of the file's content view).
3.  Copy the URL displayed in your browser's address bar. This is the direct link needed for your game.

**Example Usage in RetroCode Studios' Code Editor (Phaser.js):**
When setting up your game's assets in the `preload` function:

```javascript
function preload () {
    // Option 1: Set a base URL to simplify paths (recommended for asset packs)
    this.load.setBaseURL('[https://raw.githubusercontent.com/Gamerkong01/retrocode-studios-assets/main/](https://raw.githubusercontent.com/Gamerkong01/retrocode-studios-assets/main/)');

    // Then load your assets using paths relative to the base URL
    this.load.image('player_ship', 'SHOOTER/SpaceShooterRedux/PNG/playerShip1_blue.png');
    this.load.audio('laser_sfx', 'SHOOTER/SpaceShooterRedux/Audio/sfx_laser.wav');
    this.load.spritesheet('character_atlas', 'PLATFORMER/NewPlatformerPack/spritesheets/character_atlas.png', { frameWidth: 32, frameHeight: 32 });

    // Option 2: Load with the full raw URL if no base URL is set, or for individual assets
    // this.load.image('enemy_ship', '[https://raw.githubusercontent.com/Gamerkong01/retrocode-studios-assets/main/SHOOTER/SpaceShooterRedux/PNG/enemyRed1.png](https://raw.githubusercontent.com/Gamerkong01/retrocode-studios-assets/main/SHOOTER/SpaceShooterRedux/PNG/enemyRed1.png)');
}
