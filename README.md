# Rock-paper-scissors
import random
options=("rock","paper","scissors")
playing=True
while playing:
   player_1= None
   player_2=random.choice(options)
   while player_1 not in options:
    player_1=input("Enter your choice(rock,paper,scissors):")
   print(f"player_1:{player_1}")
   print(f"player_2:{player_2}")
   if player_1==player_2:
     print("It's a tie")
   elif player_1 =="rock" and player_2 =="scissors":
    print("player_1 win")
   elif player_1 =="paper" and player_2 =="rock":
    print("player_1 win")
   elif player_1 =="scissors" and player_2 =="paper":
    print("player_1 win") 
   else:
    print("player_2 win")
    play_again = input("WANNA PLAY AGAIN? (y/n):").lower() 
    if play_again=="y":
     playing==True
    else:
     print("******THANK FOR PLAYING********")

