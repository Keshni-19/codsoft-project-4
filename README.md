# codsoft-project-4
import random

options = ("Rock", "Paper", "Scissors")
while True:
  player = None
  computer = random.choice(options)

  while player not in options:
    player = input("Enter a choice (Rock, Paper, Scissors): ").capitalize()
  print(f"Player: {player}")
  print(f"Computer: {computer}")
  if player == computer:
    print("It's a Tie !!!")
  elif player == "Rock" and computer == "Scissors":
    print("You Win :) !!!")
  elif player == "Paper" and computer == "Rock":
    print("You Win :) !!!")
  elif player == "Scissors" and computer == "Paper":
    print("You Win :) !!!")
  else:
    print("You Lose :( !!!")

  play_again = input("Wanna play again ? (y/n): ")
  if play_again != "y":
    break
print("Thanks for playing !!!")
