# Everlasting

## 📖 Project Overview
**Everlasting** is a story-driven action game developed in **Unreal Engine 5.5.3**.  
The game follows the journey of the **first superhero in human history**, who has existed since the Middle Ages but does not know why he possesses his incredible abilities.  
As the centuries pass, **humanity evolves**, new heroes emerge, and the protagonist remains a **constant in a changing world**.  

The core of the game is an **immersive experience** with a focus on **cinematic combat, time progression, and a dynamic world that evolves around the player**.

---

## 🎮 **Core Features**
- **Seamless Time Transitions** 📜  
  The player’s **cabin** acts as a hub where time advances each time they exit the door.  
  - Uses **Level Streaming** to switch between historical epochs without loading screens.
  - The environment dynamically changes: medieval castles become modern cities.
  
- **Superhuman Abilities** 🦸  
  - **Flight** 🕊️: Initially difficult to control but improves over time.  
  - **Super Strength** 💪: Increases based on fights and environmental interactions.  
  - **Partial Invulnerability** 🛡️: Regular attacks are ineffective, but powerful forces can injure the protagonist.  
  - **No traditional XP system** 📈: Abilities evolve through **natural progression** instead of menus.

- **Cinematic Combat System** ⚔️  
  - **Physics-based attacks**: Smash enemies into walls, drag them through the ground.  
  - **Motion Matching animations** for fluid and dynamic movement.  
  - **Enemy AI that learns** and adapts to the player's combat style.  

- **Evolving World & Memory System** 🏙️  
  - The protagonist remains unchanged, but **society forgets him over time**.  
  - Old allies die, new ones emerge – the player experiences a true sense of time passing.  
  - The hero's **own memories fade**, visible only through relics and specific locations.

- **The Final Battle & Choice** 🎭  
  - The last enemy represents **the darkness of modern society** – the ultimate contrast to the protagonist’s ideals.  
  - The final confrontation determines the **fate of humanity** and the **hero’s role in the future**.  

---

## 🛠️ **Technical Details**
- **Engine:** Unreal Engine 5.5.3  
- **Rendering:** Lumen & Nanite for **real-time global illumination and high-fidelity assets**.  
- **Physics:** Chaos Physics & Physics Constraints for **realistic destruction and interaction**.  
- **Animation System:**  
  - **Motion Matching** for smooth transitions.  
  - Root Motion & Procedural Animation for seamless movement.  
- **AI System:**  
  - Utility AI + Behavior Trees for adaptive enemy combat.  
  - Dynamic Difficulty Adjustment (DDA) to challenge the player.
- **No HUD Approach:**  
  - The protagonist’s **physical state represents health** (injuries, breathing, movement).  

---

🏗️ **Project Structure**

Content/
├── Blueprints/          → Logic for gameplay, controls, AI
│   ├── Characters/      → Heroes & NPC logic
│   ├── CombatSystem/    → Melee combat, superpowers, effects
│   ├── UI/              → HUD, menus
│   ├── LevelStreaming/  → Era switching & streaming logic
│   ├── Interaction/     → Dialogue system, quick-time events
│   ├── WorldMechanics/  → Destructible objects, environmental influences
│   └── Core/            → Core game mechanics
├── Maps/                → Game worlds & levels
│   ├── HUB_Cabin/       → Main base (cabin)
│   ├── MedievalCastle/  → Medieval era
│   ├── ModernCity/      → Modern city
│   ├── FutureWorld/     → Future level
│   ├── Prototyping/     → Test level for mechanics
│   ├── Cinematics/      → Cutscene levels
│   └── Overworld/       → In case you need a large open world
├── Materials/           → Material settings
│   ├── Characters/      → Materials for the hero & NPCs
│   ├── Environment/     → Ground, buildings, objects
│   ├── Effects/         → Special effects (light effects, force fields)
│   └── UI/              → UI elements (buttons, icons)
├── Meshes/              → 3D models for characters & environment
│   ├── Characters/      → Skeletal meshes for the hero, enemies, NPCs
│   ├── Environment/     → Buildings, nature, roads, city assets
│   ├── Props/           → Items, weapons, vehicles
│   ├── Particles/       → Explosion objects, air vortices
│   └── Vehicles/        → In case planes, cars, futuristic vehicles appear
├── Textures/            → All textures for models & UI
│   ├── Characters/
│   ├── Environment/
│   ├── Effects/
│   └── UI/
├── Animations/          → Movement and combat animations
│   ├── Hero/            → Running, punching, flying animations
│   ├── NPCs/            → Enemy and civilian animations
│   ├── Combat/          → Combat animations, finishers
│   ├── Flight/          → Flight adjustments, falling, gliding phases
│   └── MotionMatching/  → In case I use UE5 Motion Matching
├── UI/                  → Menu design & interfaces
│   ├── HUD/             → Health display, special effects
│   ├── Menus/           → Pause, start screen, settings
│   ├── Dialogs/         → Dialogue windows, cinematics interface
│   ├── Inventory/       → In case I implement an item system
│   └── Icons/           → Symbols for superpowers, enemy status, etc.
├── FX/                  → Special effects with Niagara
│   ├── Superpowers/     → Flames, lightning, flight effects
│   ├── Destruction/     → Destructible objects, explosions
│   ├── Weather/         → Rain, storms, fog
│   ├── Particles/       → Blood, sand, smoke
│   └── ScreenEffects/   → Injury display, motion blur
├── Audio/               → Sound effects & music
│   ├── Music/           → Background music for levels & fights
│   ├── SFX/             → Punches, explosions, ambient noises
│   ├── UI/              → Button sounds, menu clicks
│   ├── Voices/          → Dialogues (in case voice acting is planned)
│   └── Footsteps/       → Footstep sounds depending on surface
└── Cinematics/          → In-game cutscenes
    ├── Cutscenes/       → Scripted scenes with Sequencer
    ├── DialogueScenes/  → Possible dialogue sequences
    ├── CameraAnims/     → Special camera movements
    └── MotionCapture/   → In case I use MetaHuman Animator
---

## 🚀 **Setup & Installation**
### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/YourUsername/Everlasting.git
cd Everlasting

2️⃣ Open in Unreal Engine
	•	Open Unreal Engine 5.5.3.
	•	Double-click Everlasting.uproject to open the project.

3️⃣ (Optional) Compile C++ Code

If the project includes C++ code, compile it before launching:

./GenerateProjectFiles.bat

or (for Linux/Mac):

./GenerateProjectFiles.sh

4️⃣ Play the Game
	•	Click Play inside the Unreal Editor to start testing.

📌 Development Roadmap

✅ Phase 1: Core Mechanics (3-4 months)
	•	Implement flight mechanics
	•	Build basic combat system
	•	Design first time-period (medieval setting)

✅ Phase 2: World Progression (4-6 months)
	•	Implement Level Streaming & seamless time shifts
	•	Expand enemy AI behavior
	•	Introduce memory fading & character interactions

✅ Phase 3: Final Combat & Optimization (6-12 months)
	•	Final boss encounter & player choices
	•	Motion capture integration for cutscenes
	•	Final polishing & optimization

🤝 Contributing

We welcome contributions! If you want to help:
	1.	Fork the repository
	2.	Create a new branch (feature/new-feature)
	3.	Commit your changes
	4.	Open a Pull Request

📜 License

This project is licensed under the MIT License – feel free to use and modify it.

📩 Contact & Community

For questions or collaboration, reach out:
📧 Email: tim.ms@gmx.at
💬 Discord: Everlasting Dev Server

🚀 Ready to experience the journey through time?

🔹 Clone the repo, open it in Unreal Engine, and start shaping the world of Everlasting! 🔹
