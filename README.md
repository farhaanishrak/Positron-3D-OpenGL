# Positron 3D

**Positron 3D** is a tactical 1v1 turn-based battle game set in a fully rendered 3D arena. Expanding on traditional turn-based mechanics, it introduces real-time aims, reactive defenses, and spatial positioning. Players utilize elemental abilities to manage resources and outmaneuver opponents in a dynamic combat environment.

## Game Overview

Positron combines strategic planning with reflex-based execution. The game features a multi-phase turn system where players alternate between attacking and defending, utilizing the 3D space to dodge projectiles or land critical hits.

### Key Features
* **3D Spatial Combat:** Combat outcomes depend on where attacks connect in the 3D environment, requiring players to account for trajectory and positioning.
* **Reactive Turn System:** The game is not passive; defenders must actively move, jump, or parry incoming attacks during the opponent's turn.
* **Elemental Affinity:** Players choose from six distinct elements (Fire, Water, Electric, Earth, Wind, Ice), each granting unique visual styles and status effects.
* **Dynamic Camera:** The view shifts dynamically between the attacker and defender, with an optional free-camera mode for arena exploration.
* **Dual Game Modes:**
    * **PvP:** Local multiplayer battle on a shared screen.
    * **PvAI:** Single-player mode against an adaptive AI opponent.

---

## Gameplay Mechanics

### Resources
* **HP (Health Points):** The primary survival metric; the match ends when this reaches zero.
* **ST (Stamina):** A resource required for powerful abilities. [cite_start]It recharges through successful defensive maneuvers like dodging and parrying [cite: 53-57].

### Combat System
* **Aiming:** Attacks are not auto-targeted. [cite_start]Players must time their shots using an oscillating crosshair that targets the opponent's side of the arena[cite: 21].
* **Attack Tiers:**
    * **Basic:** A standard projectile with no resource cost.
    * **Signature:** Elemental attacks that inflict status effects and follow unique trajectories.
    * **Ultimate:** High-cost, high-impact area attacks that travel along the ground.
* [cite_start]**Defense:** Defenders can move laterally to dodge, jump over ground-based attacks, or perform a timed parry to negate damage [cite: 83-85].

### Difficulty & Environment
The game scales difficulty by introducing environmental hazards:
* **Easy:** Standard arena gameplay.
* **Medium (Danger Zones):** Dynamic zones appear on the arena floor; standing in these zones negatively impacts movement speed and health.
* **Hard (Watchtowers):** Automated turrets activate on the sidelines, forcing the defender to evade additional projectiles while managing the opponent's attacks.

---

## Status Effects

Different elemental attacks apply specific status conditions that alter gameplay physics and statistics:

* **Burn (Fire):** Inflicts damage over time.
* **Freeze (Ice):** Drastically reduces movement speed, making evasion difficult.
* **Stun (Electric):** Temporarily sets health to a critical state and restricts stamina.
* **Cripple (Earth):** Increases the damage received from incoming attacks.
* **Imbalance (Wind):** Increases the speed/oscillation of the aiming crosshair, reducing accuracy.
* **Weaken (Water):** Reduces the damage output of the affected player.

---

## Controls

### General
* **P:** Pause Game.
* **Right Click:** Toggle Camera Mode (Static/Free).
* **I/K/J/L:** Move Camera (Free Mode).

### Player 1 (Red)
* **A / D:** Move Left/Right.
* **W:** Jump / Dodge.
* **Q:** Parry.
* **1 / 2 / 3:** Select Attack (Basic / Signature / Ultimate).
* **Space:** Fire Attack.

### Player 2 (Blue / AI)
* **Left / Right Arrow:** Move Left/Right.
* **Up Arrow:** Jump / Dodge.
* **Delete:** Parry.
* **1 / 2 / 3:** Select Attack.
* **Space:** Fire Attack.

---

## Installation & Requirements

Ensure you have Python installed along with the required OpenGL libraries.

```bash
pip install PyOpenGL PyOpenGL_accelerate
python "positron final.py"
