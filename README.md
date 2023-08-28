#Rock paper scissors game

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
  
