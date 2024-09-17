# Text-Based-Adventure-Game
This game was created to explore the fundamentals of adventure game development using Java. It is a text-based game that doesn't involve a graphical user interface (GUI), yet remains fun and engaging to both create and play.
The premise is that the main character enters a dungeon and randomly encounters four types of enemies: a skeleton, a zombie, a warrior, and an assassin. The hero starts with 3 health potions and can potentially find more after defeating enemies. Players can choose to attack, use a potion, or run during each encounter. This project serves as a great introduction to game development concepts in Java.
Based on the provided code, here’s a theoretical explanation of the text-based adventure game:

---

This text-based adventure game is written in Java and involves a dungeon-crawling hero who encounters random enemies. The game is controlled through user input, allowing the player to take specific actions during their encounters with enemies.

#### **Key Concepts and Structure**

1. **Game Setup:**
   - The game uses Java's `Random` class to simulate random enemy encounters and combat outcomes.
   - The `Scanner` class is used to take input from the player, allowing them to decide their next action.

2. **Game Variables:**
   - **Enemies**: There are four different enemies that can appear: *Skeleton*, *Zombie*, *Warrior*, and *Assassin*.
   - **Player Stats**: 
     - The player starts with 100 health points.
     - They can deal a maximum of 50 damage per attack.
     - The player also starts with 3 health potions, each of which restores 30 health points.
   - **Enemy Stats**: 
     - Enemies can have up to 75 health points.
     - They can deal up to 25 damage per attack.

3. **Game Flow:**
   - The game continuously runs in a loop until the player either decides to quit or dies.
   - **Enemy Encounter**: On each iteration, a random enemy appears with a random amount of health (up to 75 points).
   - **Player Actions**:
     - **Attack**: The player can attack the enemy, dealing a random amount of damage (up to 50). The enemy also counterattacks, dealing random damage to the player (up to 25).
     - **Drink Health Potion**: The player can heal themselves by drinking a potion, restoring 30 health points. However, potions are limited, and the player starts with only 3.
     - **Run**: The player has the option to run away from the battle, moving on to the next encounter.

4. **Combat Mechanics:**
   - During combat, both the player and the enemy take turns inflicting damage on each other. The enemy's health decreases with each attack, and if the player’s health drops below 1, the game ends.

5. **Potion Drops:**
   - After defeating an enemy, there’s a 50% chance the player will find a health potion, which is added to their inventory for future use.

6. **Game Over Conditions:**
   - The game ends if the player’s health is reduced to zero or if they choose to quit.

---
