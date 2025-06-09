# Rock-Paper-Scissor-Game-in-Python
import random
options=("rock","paper","scissor")
running=True
while running:
    player=None
    computer=random.choice(options)    
    if player not in options:
        player=input("Enter the choice(rock,paper,scissor):").lower()
    print(f"player:{player}")
    print(f"Computer:{computer}")
    if player==computer:
        print("Its a tie!")
    elif player=="rock" and computer=="scissor":
        print("You win!")
    elif player=="paper" and computer=="rock":
        print("You win!")
    elif player=="scissor" and computer=="paper":
        print("You win!")
    else:
        print("You lose the game!")
    play_again=input("play_again(y/n)?:").lower()
    if play_again!="y":
        running=False
print("Thanks for playing...")
