# Game-s
Rock_paper_scissors 
import random

choices = ["rock", "paper", "scissors"]

user = input("Enter rock, paper or scissors: ").lower()
computer = random.choice(choices)

print("You chose:", user)
print("Computer chose:", computer)

if user == computer:
    print("It's a draw!")
elif (user == "rock" and computer == "scissors") or \
     (user == "paper" and computer == "rock") or \
     (user == "scissors" and computer == "paper"):
    print("You win!")
else:
    print("Computer wins!")
