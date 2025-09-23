WOCI Games Test Task: Mini Survival Gameplay Prototype

Project Overview
This project is a mini survival gameplay prototype built using Unreal Engine 5. The objective was to create a small first-person scenario demonstrating core game development skills, including player systems, AI behavior, and environmental design.
The prototype features a basic first-person character who navigates a small environment. The player must avoid a patrolling enemy AI and can collect items to interact with the world.


Implemented Features
Player System
First-Person Movement: Implemented standard first-person controls (WASD for movement and Space for jumping).
Health System: The player starts with 100 health. This value decreases when the player is attacked by the enemy AI.

Enemy AI
Behavior Tree Logic: The enemy AI uses a Behavior Tree to manage its state.
Patrol: The enemy patrols a set path of points within the level.
Chase: When the player enters the enemy's perception range, the AI will stop patrolling and chase the player.
Attack: If the player is within attack range, the enemy will stop chasing and attack the player, reducing their health.
Return to Patrol: If the player escapes the enemy's perception range, the AI will return to its last known patrol point and resume patrolling.
Death: The enemy is set to disappear once its health reaches zero.

Environment & Level Design
Safe Zone: A designated area where the enemy AI will not enter, providing the player with a brief respite.
Danger Zone: The main area of the level where the enemy AI patrols.

C++ and Blueprint Implementation Breakdown
Due to time constraints, this prototype was primarily developed using Unreal Engine's Blueprint visual scripting system. The core logic for player movement, health, AI behavior, and level interactions is built entirely within Blueprints.

Blueprints:
Player Character: All player movement, camera controls, and health system logic are handled in the BP_PlayerCharacter Blueprint.
Enemy AI: The Behavior Tree and AI Controller logic for the enemy's patrol, chase, and attack states are managed in Blueprints. This includes the AI's perception system (AIPerceptionComponent) and its ability to reduce the player's health.
Game Mode & UI: The BP_GameMode handles the overall game flow, and the user interface (UI) elements for health display were created using Widget Blueprints.

C++:
No C++ classes were created for this submission. The project relies on the core functionality provided by the base C++ classes of Unreal Engine.
This approach demonstrates proficiency in leveraging Unreal Engine's native tools and a strong understanding of Blueprint-based game logic and state management.

Unimplemented Requirements
I want to be upfront about the requirements I was unable to complete within the given timeframe.
Inventory System: The player's ability to collect and use items (Food and Tool) was not implemented.
Combat System: The player's attack functionality, which was dependent on collecting the Tool, is not present.
Day/Night Cycle: The bonus task of implementing a day/night cycle that affects enemy aggression was not added.
Despite these omissions, the current prototype effectively demonstrates the foundational skills in AI and gameplay systems requested in the assignment. I am confident in my ability to implement these features and integrate them with the existing Blueprint logic.



How to Run the Project
1.Clone or download the project from the provided GitHub link.
2.Open the project in Unreal Engine 5.3 or later.
3.Open the TFPMovement folder located in the Maps folder and open the DemoLevel.
4.Press "Play" to start the game and experience the prototype.

Thank you for your consideration. I look forward to discussing my project further with the team.

