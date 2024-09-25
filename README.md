# Adventure in C

## Objective
Create a C program that creates a simple text-based adventure game like old school [Zork](https://en.wikipedia.org/wiki/Zork). The player should navigate through a series of rooms, make decisions, and manage a basic inventory. This assignment will demonstrate your understanding of variables, data types, user input, conditional statements, loops, and basic logic.

## Requirements

1. Create a game with at least five different "rooms" or scenarios.
2. Allow the player to move between rooms and make decisions using numerical menu options.
3. Implement a simple inventory system where the player can collect and use items.
4. Include at least three items they player can collect and use in specific scenarios.
5. Implement a win condition and at least one lose condition.
6. Display the player's current status (current room, inventory) after each action.
7. Use appropriate data types for different elements of the game.
8. Implement input validation to ensure the player enters valid choices.

### Example Game Structure
**Room 1 (Start): Dark Cave**


Options:
1. Go deeper,
2. Search for a light source

*Item:* Torch (if searched)


**Room 2: Underground Lake**

Options:
1. Swim across
2. Look for another way

*Item:* Key (if looked for another way)

**Room 3: Ancient Temple**
Options:
1. Examine statue
2. Open door (requires Key)
   
*Item:* Amulet (if statue examined)

**Room 4: Treasure Room**
Options:
1. Take treasure
2. Leave treasure
   
*Win condition:* Take treasure while having Amulet

*Lose condition:* Take treasure without Amulet.

**Room 5: Exit**
Options:
1. Leave cave
2. Go back
   
*Win condition:* Leave cave with treasure.

---
### Gameplay Example:

Welcome to the Creeptastic Cave Adventure!

You find yourself in a dark cave. What do you want to do?
1. Go deeper
2. Search for a light source
Enter your choice (1-2): 2

You found a torch! I've added it to your inventory.

Your Current Status
Location: Dark Cave
Inventory: Torch

What do you want to do?
1. Go deeper
2. Search for a light source
Enter your choice (1-2): 1

You proceed deeper into the cave and reach an underground lake.
What do you want to do?
1. Swim across
2. Look for another way
Enter your choice (1-2):

---

### Project Hints
- Use integers to represent rooms and player choices.
- Use an array or individual variables to represent the player's inventory. We haven't learned arrays yet, so try it on your own if you dare.
- Implement a main game loop that continues until a win or lose condition is met.
- Use if-else chains to handle different rooms and choices.
- Remember to include the necessary header files: #include <stdio.h>
- Use the CS50 library for user input and printf() for output.

*Bonus Challenges*
- Add simple puzzles that require combining inventory items.
- Implement a basic combat system with a health stat for encounters with cave creatures.
- Create multiple paths to win, with different endings based on the player's choices and inventory.
