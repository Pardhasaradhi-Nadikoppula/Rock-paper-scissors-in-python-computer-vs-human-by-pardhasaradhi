Rock-Paper-Scissors Game
A simple Python implementation of the classic Rock-Paper-Scissors game, where you can play against the computer.

Table of Contents
Introduction
How to Play
Installation
Usage
Contributing
License
Introduction
This is a Python implementation of the Rock-Paper-Scissors game, a popular hand game played between two people. In this version, you can play against the computer, which makes a random choice.

How to Play
Clone or download this repository to your local machine.

Open a terminal or command prompt and navigate to the project directory.

Run the rps_game.py script using the following command:

shell:
***********************************************************************************************************
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

#Write your code below this line 👇
import random

humanchoice = input("what do you choose, Type 0 for Rock, 1 for Paper and 2 for Scissors")

game = [rock, paper, scissors]

pick = random.choice([rock, paper, scissors])

if humanchoice == "0":
  print(f"{rock}")
  print(f"computer choice:\n {pick}")
  if pick == game[0]:
    print("it's a Tie break!!")
  if pick == game[1]:
    print("You won!!")
  if pick == game[2]:
    print("You won!!")

if humanchoice == "1":
  print(f"{paper}")
  print(f"computer choice:\n {pick}")
  if pick == game[0]:
    print("You won!!")
  if pick == game[1]:
    print("it's a Tie break!!")
  if pick == game[2]:
    print("You lost the game!!")

if humanchoice == "2":
  print(f"{scissors}")
  print(f"computer choice:\n {pick}")
  if pick == game[0]:
    print("You lost the game!!")
  if pick == game[1]:
    print("You won!!")
  if pick == game[2]:
    print("it's a Tie break!!")
  ********************************************************************************************************************************

Follow the on-screen instructions to select your choice (rock, paper, or scissors).

The computer will randomly choose its move, and the winner of the round will be displayed.

Installation
Make sure you have Python 3.x installed. If not, you can download it from the official Python website: Python Downloads.

Clone this repository to your local machine using Git:

shell


python rps_game.py
Follow the on-screen instructions to play the game.

Contributing
If you would like to contribute to this project, you can:

Fork the repository.
Make your improvements or changes.
Submit a pull request describing your changes.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Feel free to customize this template according to your project's details and your preferred writing style. You can add more sections or information if needed. The goal is to make it clear and easy for others to understand and use your Rock-Paper-Scissors game.
