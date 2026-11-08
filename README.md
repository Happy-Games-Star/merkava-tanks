# Merkava Come Back - Tanks Battle 🪖👑

A retro-inspired **tank battle** game with a bold cartoon arena look. Drive your Merkava tank, protect the crown tower and destroy every enemy tank across **10 levels** and **3 difficulty modes**. One HTML file, no dependencies, no build step.

**[▶ Play online](https://happy-games-star.github.io/merkava-tanks/)**

## The idea

Enemy tanks roll in from the top of the screen in waves. They hunt for your crown tower at the bottom. Destroy all of them before the tower falls or you run out of lives. Clear all 10 levels to bring the Merkava back.

## Features

- Single-player campaign with **10 levels**, a different map on every level
- **3 difficulty levels:**
  - **Easy:** 5 lives, slower and fewer enemies
  - **Normal:** 3 lives
  - **Hard:** 2 lives, more and faster enemies that target the tower more often
- Three enemy types: basic (red), fast (orange, from level 3), armored (purple, from level 5, takes several hits)
- Destructible bricks, indestructible steel, bushes that hide tanks, water that blocks movement
- Short shield after you lose a life
- Score, lives and enemies-left display, with a bonus for remaining lives after each level
- Best score saved in the browser for each difficulty
- Retro sound effects generated in the browser, no audio files
- Built-in **How to play** screen that also pauses the game
- Works on desktop and mobile: keyboard controls, or on-screen D-pad and fire button on touch devices

## Controls

| Action | Computer | Phone / tablet |
| --- | --- | --- |
| Drive | Arrow keys or WASD | On-screen arrow buttons |
| Fire | Space (hold to keep firing) | FIRE button |

## Tips

- Bricks around the tower are your only shield. Do not shoot them.
- Steel walls cannot be destroyed, so go around them.
- Armored tanks flash a lighter color when damaged.
- Bushes hide enemies too, so watch the edges.

## Run locally

No installation needed. Download the repository and open `index.html` in any modern browser.

```bash
git clone https://github.com/Happy-Games-Star/merkava-tanks.git
cd merkava-tanks
# then open index.html in your browser
```

## Deploy with GitHub Pages

1. Open **Settings → Pages**.
2. Under **Source**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
3. Save. The game goes live at `https://happy-games-star.github.io/merkava-tanks/`.

## Tech

- HTML5 Canvas, CSS3 and vanilla JavaScript
- Web Audio API for sound effects
- Seeded random map generation, so each level always has the same layout
- [Lilita One](https://fonts.google.com/specimen/Lilita+One) from Google Fonts, with a system font fallback when offline

## Customization

- **Difficulty:** edit the `DIF` object in the script (lives, enemy speed, fire rate, enemies on screen, enemy count).
- **Colors:** change the CSS variables at the top of the `<style>` block.
- **Level layouts:** change the density numbers inside `genMap()`.

## Disclaimer

This is an unofficial, fan-style project. Its gameplay is inspired by classic 8-bit tank games and its look by mobile arena games. It is not affiliated with or endorsed by Supercell, Namco or any other company, and it uses none of their logos, characters, artwork or music.

## License

Released under the [MIT License](LICENSE). Add a `LICENSE` file when you create the repository, or choose another license.
