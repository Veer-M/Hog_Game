# Hog Dice Game

This project involves the development of a simulator and multiple strategies for the dice game Hog. The goal is to implement various game rules and strategies using control statements and higher-order functions.

## Rules

In Hog, two players take turns trying to be the first to reach a total score of at least 100. Here are the basic rules:

- On each turn, the current player chooses the number of dice to roll, up to a maximum of 10.
- The player's score for the turn is the sum of the dice outcomes.
- If any of the dice outcomes is a 1, the player's score for the turn is 1 (Pig Out).

In addition to the basic rules, there are some special rules:

- Free Bacon: A player who chooses to roll zero dice scores k+3 points, where k is the nth digit of pi after the decimal point, and n is the total score of their opponent. If the opponent's score is 0, k is 3.
- Swine Align: If both players have a positive score and the Greatest Common Divisor (GCD) of the current player's score and the opponent's score is at least 10, the current player takes another turn.
- Pig Pass: If the current player's score is lower than the opponent's score and the difference between them is less than 3, the current player takes another turn.
  
## Project Structure

The project contains the following main files:

- hog.py: The main implementation file for Hog. This is where you'll complete most of your code.
- dice.py: Contains functions for rolling dice.
- hog_gui.py: A graphical user interface (GUI) for playing Hog (Uses default_graphics.py).
- ucb.py: Utility functions.
- calc.py: Calculates and compartes the win rate of two different strategies in the game of Hog.
