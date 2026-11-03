# 🧟 Zombie Survival Game

> A third-person survival shooter developed with **Unity 6**, where the player must survive relentless zombie attacks until a rescue helicopter arrives. Zombies continuously spawn around the player, forcing quick decision-making, accurate shooting, and constant movement to stay alive.

> **⚠️ This project was developed for educational purposes as part of a university coursework assignment.**

---

## 🎮 Gameplay

The player is stranded in a dangerous area overrun by zombies. The objective is simple but challenging:

* Survive for **180 seconds**
* Eliminate approaching zombies before they overwhelm you
* Wait for the rescue helicopter to land
* Enter the helicopter after its doors open to complete the mission

The player loses if their health reaches zero before evacuation.

---

## ✨ Features

* 🎯 Third-Person Shooter (TPS) gameplay
* 🕹️ Smooth WASD character movement
* 🖱️ Mouse-controlled camera system
* 🎯 Crosshair aiming system
* 🔫 Left-click shooting mechanic
* 🧟 AI-controlled zombies that chase the player
* ❤️ Health and damage system
* 💀 Enemy elimination system
* 📈 Continuous enemy spawning
* 🎭 Randomized zombie walking animations
* 🚁 Rescue helicopter landing sequencegi
* 🚪 Helicopter door opening animation
* ⏱️ 180-second survival objective
* 🏆 Victory and Game Over conditions
* 🖥️ On-screen gameplay UI and status messages

---

## 🧠 Game Systems

### Player Controller

The player uses a third-person movement system controlled by keyboard input, while the camera follows the player using mouse movement. Character animations are managed through Unity's Animator State Machine.

### Enemy AI

Zombies are implemented using a custom AI system based on **CharacterController** and vector calculations instead of Unity NavMesh. Every spawned zombie continuously tracks the player's position and attempts to reach them.

To improve visual variety, each newly spawned zombie is assigned one of several different walking/chasing animations at random.

### Combat System

Players can aim using the center crosshair and shoot zombies with the left mouse button. Each zombie has its own health value and disappears from the scene when defeated.

### Spawn Manager

The game continuously generates new zombies around the player's surroundings during gameplay, maintaining constant pressure throughout the survival period.

### Win & Lose System

The objective is not simply eliminating zombies—it is surviving.

After **180 seconds**, a rescue helicopter arrives and performs a landing sequence created with Unity animations. Once the helicopter has completely landed, its doors open and become accessible.

The player wins only by successfully entering the helicopter after the doors have opened. If the player dies before evacuation, the game pauses and displays a **"You Died"** screen.

---

## 🛠️ Technologies Used

* Unity 6
* C#
* Unity Animator State Machine
* CharacterController
* Custom Enemy AI
* Unity Physics
* Prefab System
* UI System
* Particle & Animation Systems

---

## 📂 Project Structure

```text
Assets/
    ├── TheGame/
        ├── Materials/
        ├── Models/
        ├── Prefabs/
        ├── Scripts/
        ├── Textures/
```

---

## 🚀 Getting Started

### Requirements

* Unity 6 or newer

### Installation

```bash
git clone https://github.com/yourusername/zombie-survival.git
```

Open the project using Unity Hub and load the main scene.

Press **Play** to start surviving.

---

## 📸 Screenshoots

> Helicopter Landing

<img width="1290" height="913" alt="helicopter-landing" src="https://github.com/user-attachments/assets/c24bfd4a-21fc-48c8-94b0-65a3058f1d52" />

---

> Zombie Chasing

<img width="1156" height="817" alt="zombie-chasing" src="https://github.com/user-attachments/assets/d505e07e-2cba-40e5-8499-b6a2b5bf1daf" />

---

> Win Screen (Reached to Helicopter)

<img width="1290" height="912" alt="win-screen" src="https://github.com/user-attachments/assets/7258287f-91a0-41d9-99cc-2fb1ed0f8938" />

---

> Lose Screen (Died by Zombie)

<img width="1133" height="826" alt="lose-screen" src="https://github.com/user-attachments/assets/646416d3-db01-4c25-9fb4-2485454bc593" />

---

## 📸 Gameplay Video

> Youtube

```
https://www.youtube.com/watch?v=tqdqDnNu7aE
```

---

## 🎯 Controls

| Action | Key               |
| ------ | ----------------- |
| Move   | WASD              |
| Aim    | Mouse             |
| Shoot  | Left Mouse Button |
| Jump   | Space             |

---

## 📚 Learning Outcomes

This project helped reinforce practical game development concepts including:

* Third-person character controllers
* Camera systems
* AI behavior using vector mathematics
* Object-oriented programming in Unity
* Enemy spawning systems
* State machine animations
* Health and damage mechanics
* Gameplay loop design
* Win/Lose state management
* Prefab-based architecture

---

## 👨‍💻 Author

**Mert Akdemir**

Software Engineer | Backend Developer (.NET & Node.js) | Database Engineer

If you like this project, consider giving it a ⭐ on GitHub.
