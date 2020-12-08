# Ithaca-Project2020

1. [Introduction and background of the project](#Introduction-and-background-of-the-project)
2. [Storytelling](#Storytelling)
3. [How to play](#How-to-play)
4. [Code structure](#Code-structure)
5. [Bugs and things to fix](#Bugs-and-things-to-fix)
6. [Improvement ideas](#Improvement-ideas)

------------------------

## Introduction and background of the project

This game started to be developed in a C++ development course at the end of my 2nd year of engineering school (June 2020). The instruction was to "Develop a game based on an episode of Greek mythology" in two weeks and in pairs. The game is coded in C++ and uses SFML in particular. 
As I really liked developing this game, I personally decided to resume its development and improve it in order to develop more C++ development skills.
I started to resume the development of the game on 10/10/2020 and the first commit corresponds to the first phase of the project which was to make the game start, work and end pretty much correctly. This first commit was made on 10/23/2020.

------------------------

## Storytelling

"After a long journey back from the Trojan War, Ulysses finally approaches the coast of Ithaca, the island of which he is king. But beware, sirens are also roaming in these waters, they could capsize Ulysses' boat before he reaches port..."

This game is a 1 vs 1 game played on the same machine. One player interprets Ulysses and his fleet, the other one interprets the sirens.

### Rules of the game

#### Ulysses
  
  * **Player's goal :** to make reach the island of Ithaca to the boat on which Ulysses is located
  * **Beginning of the game round :** 
      * the boats of Ulysses' fleet are randomly placed on the edges of the map
      * the magenta boat is the one with Ulysses on it
  * **Course of a game round :**
      * choice of the boat on which to place Ulysses (only during the first round of the game)
      * *choice between two actions to be carried out*
          * move each of his boats by only one square
          * move only one of its boats with a single roll of the dice
      * *intervention of the gods*
          * malus or bonus (examples: you can move 2 times further, you can move a maximum of 2 squares)
          * random and different for each round of the game
      * relocation of the boat(s), taking into account divine intervention
  * **Victory if :** the ship on which Ulysses is is on a square representing the island of Ithaca at the end of the turn
    
#### Sirens

* **Player's goal :** to sink the boat on which Ulysses is on before he reaches Ithaca
* **Beginning of the game round :**
  * the sirens are on a square representing the island of Ithaca (in the center of the map for the moment)
* **Course of a game round :**
    * receiving information about the position of Ulysses' boats: for each of the boats, the player knows in which quarter of the field that boat is located, thanks to the cardinal points (the sirens can feel the movement of the waves)
    * choice of a square on the map where the sirens will be sent to attack Ulysses' ships (the attack zone is induced from the information retrieved at the previous point)
    * if the chosen destination corresponds to a square on which a boat from Ulysses' fleet is located, this boat is sunk: it disappears from the map and from Ulysses' fleet
* **Victory if :** the destination chosen corresponds to the square on which the boat on which Ulysses is on is located

------------------------

## How to play

------------------------

## Code structure

------------------------

## Bugs and things to fix

------------------------

## Improvement ideas

------------------------
