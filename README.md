# WOCI Games Test Task: Mini Survival Gameplay Prototype

## 🎮 Project Overview
This project is a **mini survival gameplay prototype** built using **Unreal Engine 5.3**.  
The objective was to create a small first-person scenario demonstrating core game development skills, including:

- Player systems  
- AI behavior  
- Environmental design  

The prototype features a **first-person player** who navigates a small environment, avoids a patrolling enemy AI, and interacts with the world.

---

## ✅ Implemented Features

### Player System
- **First-Person Movement**: Standard FPS controls (`WASD` for movement, `Space` for jump).  
- **Health System**: Player starts with **100 health**, reduced when attacked by the enemy.  

### Enemy AI
- **Behavior Tree Logic**:
  - **Patrol**: Enemy follows a set path.  
  - **Chase**: Detects and follows the player if within perception range.  
  - **Attack**: Damages the player if within attack range.  
  - **Return to Patrol**: Resumes patrol if the player escapes.  
  - **Death**: Enemy disappears when its health reaches `0`.  

### Environment & Level Design
- **Safe Zone**: Area where the enemy AI will not enter.  
- **Danger Zone**: Main playable area patrolled by the enemy.  

---

## ⚙️ C++ vs Blueprint Breakdown

### Blueprints
- **Player Character**: Movement, camera, and health system (`BP_PlayerCharacter`).  
- **Enemy AI**: Behavior Tree, AI Controller, and Perception (`AIPerceptionComponent`).  
- **Game Mode & UI**: Game flow handled in `BP_GameMode`, with health UI in Widget Blueprints.  

### C++
- **No custom C++ classes** were created for this submission.  
- Relies on **Unreal’s base C++ classes** with all gameplay logic implemented in Blueprints.  

---

## 🚧 Unimplemented Features
The following were not completed due to time constraints:
- **Inventory System**: Item collection (Food & Tool).  
- **Combat System**: Player attack functionality (dependent on Tool).  
- **Day/Night Cycle**: Bonus feature to affect enemy aggression.  

> These features can be added and integrated with the existing Blueprint systems if required.

---

## ▶️ How to Run the Project
1. **Clone or download** the repository.  
2. Open the project in **Unreal Engine 5.3 or later**.  
3. Navigate to: Content/Maps/TFPMovement/DemoLevel.umap
4. Press **Play** to start the game.  

---
