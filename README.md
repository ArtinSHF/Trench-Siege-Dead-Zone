# Trench Siege — Dead Zone 🧟

<img width="1917" height="892" alt="Screenshot" src="https://github.com/user-attachments/assets/78dce5f1-b508-49bb-afe9-be851c50cb89" />->

---

Trench Siege — Dead Zone is a browser-based zombie tower defense game featuring endless enemy waves, a customizable defensive arsenal, branching upgrades, tactical abilities, permanent research progression, and procedurally rendered battlefields.

Choose your map, establish a defensive line, and hold back an increasingly dangerous outbreak using infantry, artillery, experimental weapons, support emplacements, and a leveling Hero Commander.

Built as a single-file web game, the project combines real-time combat simulation, custom Canvas rendering, synthesized audio, and persistent progression without relying on a dedicated game engine.

## 🌐 Live Website

**Live site:** https://trench-siege-dead-zone.vercel.app/

---

## 🎮 About the Project

The objective is simple: keep the dead from breaking through your defenses for as long as possible.

Enemies follow a winding battlefield route while your emplacements automatically acquire targets and attack. Each successful defense earns money for additional units and upgrades.

As the waves advance, enemy health and overall threat increase, introducing tougher encounters that demand stronger defenses and better positioning.

Between runs, Research Points unlock permanent improvements to your economy, firepower, and starting defenses.

---

## 🚀 Features

### Endless Survival & Battlefield Selection

* **Endless Waves:** Face escalating enemy strength with no fixed final wave.
* **Three Battlefields:**
  * **Muddy Trenches:** A winding trench line through muddy terrain.
  * **Ruined Outpost:** A rubble-covered defensive route.
  * **Bunker Complex:** Tight turns through concrete defensive corridors.
* **Four Difficulty Levels:** Easy, Normal, Hard, and Nightmare.
* **Wave Controls:** Start waves manually or enable automatic progression.
* **Fast-Forward:** Cycle simulation speeds to accelerate combat.

### Defensive Arsenal

Deploy 10 different unit types, each with its own combat role:

| Unit | Role |
| :--- | :--- |
| Rifle Squad | Flexible infantry defense |
| Heavy MG | Sustained fire against crowds |
| Sniper Nest | Long-range, high-damage attacks |
| Mortar Team | Explosive bombardment |
| Flamethrower | Close-range fire and burning damage |
| Laser Post | Advanced energy-based defense |
| Tesla Coil | Electrical attacks |
| Napalm Cannon | Incendiary area denial |
| Support Post | Support effects and defensive synergies |
| Hero Commander | Experience-based combat progression |

### Upgrades & Targeting

* **Three Upgrade Paths per Emplacement:** Specialize units through distinct development branches.
* **Five Tiers per Path:** Unlock increasingly powerful weapons and enhancements.
* **Visual Progression:** Emplacement artwork changes as upgrades are purchased.
* **Target Priorities:** Switch between First, Last, Strong, and Close.
* **Specialized Effects:** Build around armor piercing, splash damage, burning, slowing, stealth detection, and support bonuses.
* **Economic Options:** Certain upgrades provide recurring income alongside combat improvements.

### Tactical Abilities

* **Tactical Airstrike:** Strike a selected area with explosive damage.
* **Reinforce Barrier:** Temporarily obstruct the enemy advance.
* **Fuel Drum:** Place an explosive drum that detonates after a short fuse.
* **Electric Fence:** Deploy a temporary electrical damage zone.
* **Spike Trap:** Damage and slow enemies entering its trigger area.
* **Cooldown Management:** Time abilities carefully during difficult waves.

### Enemies & Boss Encounters

* **Varied Enemy Classes:** Fight shamblers, sprinters, crawlers, armored enemies, spitters, and other specialized threats.
* **Defensive Traits:** Some enemies use armor, shields, low profiles, or burrowing mechanics.
* **Death Effects:** Certain infected release hazardous gas when killed.
* **Boss Enemies:** Face heavy threats such as Mutants and Behemoths.
* **Escalating Pressure:** Enemy durability scales as the run progresses.

### Hero Commander

* **Experience & Leveling:** The Hero Commander gains experience during combat.
* **Automatic Stat Growth:** Levels improve damage, range, attack speed, and other capabilities.
* **Evolving Appearance:** The commander’s visual presentation develops with progression.

### Permanent Research & Achievements

* **Research Points:** Earn progression currency from normal survival runs.
* **Permanent Tech Tree:** Purchase upgrades across three categories:
  * Economy
  * Combat
  * Survival
* **Persistent Bonuses:** Improve starting cash, tower costs, wave rewards, attack speed, damage, and starting lives.
* **Achievements:** Unlock milestones tied to combat and progression.
* **Lifetime Statistics:** Track kills, boss defeats, cash earned, highest wave, and unit construction.
* **Local Saving:** Progression is stored in the browser using localStorage.

### Sandbox & Development Tools

* **Unlimited Cash:** Experiment with expensive builds.
* **Infinite Health:** Test defenses without losing to enemy leaks.
* **Wave Selection:** Jump directly to a chosen wave.
* **Enemy Spawning:** Spawn enemy types and bosses for testing.
* **Progression Safeguard:** Using development tools marks the run as sandbox-tainted and disables Research Point rewards.

### Visuals & Audio

* **Procedural Canvas Artwork:** Terrain, units, enemies, and combat effects are drawn in code.
* **Dynamic Weather:** Changing battlefield conditions and atmospheric effects.
* **Particle Effects:** Explosions, sparks, smoke, fire, and electrical effects.
* **Combat Feedback:** Floating text, screen shake, flashes, and targeting indicators.
* **Synthesized Sound:** Weapon effects and background music generated through the Web Audio API.

---

## 🛠 Tools & Technologies Used

* **HTML5:** Application structure and Canvas element.
* **CSS3:** Battlefield interface, menus, panels, and visual styling.
* **JavaScript:** Combat logic, upgrades, wave generation, progression, and input handling.
* **Canvas 2D API:** Procedural terrain, animated units, projectiles, and effects.
* **Web Audio API:** Synthesized sound effects and music.
* **localStorage:** Permanent research, achievements, and lifetime statistics.

The core game does not require a frontend framework, backend server, or dedicated game engine.

---

## ▶️ How to Run Locally

The game is contained in a single HTML file.

### Quick Start

Open `trench-siege-dead-zone.html` in a modern browser.

### Recommended Development Method

1. Open the project folder in VS Code.
2. Install the **Live Server** extension.
3. Right-click `trench-siege-dead-zone.html`.
4. Select **Open with Live Server**.

No package installation or build step is required.

For static hosting, the game file can be renamed to `index.html`.

---

## ⌨️ Controls

| Input | Action |
| :--- | :--- |
| Click an arsenal unit, then click the battlefield | Place an emplacement |
| Click an existing emplacement | Inspect and upgrade it |
| Click an ability, then click the battlefield | Deploy the selected ability |
| Spacebar | Start the next wave |
| F | Cycle fast-forward speed |
| A | Toggle automatic waves |
| Escape | Cancel placement or targeting; close supported overlays |

---

## 💾 Save Data

Permanent progression is saved locally in your browser.

This includes Research Points, purchased research, achievements, and lifetime statistics.

Returning to the main menu abandons the current run. Permanent progression is separate from an active battlefield session.

Clearing browser storage or using **Reset Save Data** removes saved progression. Saves are not synchronized between browsers or devices.

---

## 📁 Project Structure

Current single-file layout:

```text
trench-siege-dead-zone/
└── trench-siege-dead-zone.html
```

The HTML file contains the interface, styles, game logic, rendering systems, audio, and progression systems.

---

## 📌 Status

Playable single-file browser game featuring endless survival, permanent progression, achievements, and sandbox testing tools.

**Deployment:** Deployed using vercel

---

## 🧠 Technical Takeaways

This project demonstrates:

* **Real-Time Simulation:** Coordinating waves, enemies, projectiles, damage, traps, and cooldowns.
* **Procedural Rendering:** Creating detailed battlefields and evolving unit artwork with Canvas.
* **Data-Driven Design:** Defining units, enemies, upgrades, and research through reusable configuration objects.
* **Persistent Progression:** Separating temporary run state from permanent research and achievements.
* **Performance Management:** Reusing objects through pools and caching rendered artwork.
* **Browser Audio Synthesis:** Producing combat feedback without a conventional sound-asset pipeline.
* **Testing Tools:** Building sandbox controls for balance testing and late-game experimentation.

---

## ⚠️ Note

Trench Siege — Dead Zone is a fictional zombie survival strategy game.

Progression is stored locally, and sandbox runs are separated from normal Research Point rewards.
