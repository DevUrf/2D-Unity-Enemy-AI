# 🧠 Enemy AI for Unity

This repository contains a complex 2D enemy AI system for Unity, designed to give enemies various behaviors such as patrolling, chasing, attacking, evading, retreating, and more. The AI state transitions based on proximity to the player and other conditions like health, line of sight, and attack range. This script is ideal for games that require sophisticated enemy behavior with dynamic state changes.

## 🚀 Features

- **AI States**: 
  - 🕵️‍♂️ **Patrolling**
  - 🏃‍♂️ **Chasing**
  - 🥊 **Attacking**
  - 🌀 **Evading**
  - 🧘‍♂️ **Idle**
  - 🚨 **Alert**
  - 🏃 **Retreating**
  - 🏃‍♂️💨 **Fleeing**

- **Customizable Behavior**:
  - 🏃 **Adjustable movement speeds** for patrolling and chasing.
  - 📍 **Patrol points** to define enemy patrol path.
  - ⚔️ **Ability to attack** the player when in range.
  - 🔄 **Dynamic evasion behavior** when the enemy gets too close to the player.
  - ⬆️ **Retreat behavior** when the enemy's health is low.
  - 💔 **Fleeing behavior** when health is critically low.

- **Health and Combat**:
  - ❤️ The enemy has **health** that can be depleted when taking damage.
  - 💪 **Health-based transitions** (retreat or flee) for more tactical enemy behavior.

- **Sight and Range**:
  - 👀 **Detection range** for chasing and alerting based on proximity to the player.
  - 📏 **Customizable sight range, evade range, and aggro range** for different difficulty levels.

## 📥 Installation

1. **Download the script**:
   - Download the `Enemy.cs` script from the repository.

2. **Add to Unity Project**:
   - Place the `Enemy.cs` script in your Unity project's `Scripts` folder.

3. **Create Enemy GameObject**:
   - Create a new GameObject (e.g., `Enemy`) in your Unity scene.
   - Attach the `Enemy.cs` script to the GameObject.

4. **Assign Patrol Points**:
   - Assign patrol points (empty GameObjects) to the `Patrol Points` array in the Unity Inspector to define the enemy's patrol path.

5. **Set Player Tag**:
   - Make sure your player GameObject has the `Player` tag for detection.

6. **Customize AI Settings**:
   - Adjust the variables in the Inspector, such as movement speed, attack range, health, and detection range to fit your game's difficulty and design.

## 🧑‍💻 Example Use

```csharp
// You can call the TakeDamage method to deal damage to the enemy:
enemy.TakeDamage(10f);  // Deals 10 damage to the enemy
