Skip to content
onyangoadrian
/
onyangoadrian
Code
Pull requests
Actions
Projects
Security
Insights
Settings
onyangoadrian/.github/workflows/python-package.yml
@onyangoadrian
onyangoadrian Create python-package.yml
 1 contributor
45 lines (35 sloc)  1.27 KB
from tkinter import *

root=Tk()
root.geometry('400x400')
root.title("Rock Paper Scissors Game")


button1 = Button(text="       Rock       ",bg="sky blue")
button1.grid(column=0,row=1)
button2 =Button(text="       Paper      ",bg="pink")
button2.grid(column=0,row=2)
button3 =Button(text="      Scissor     ",bg="light green")
button3.grid(column=0,row=3)
button4=Button(text="    play ",bg="purple",)
button4.grid(column=3,row=3)
root.mainloop()



import random
user_action=input("Enter a choice (rock, paper, scissors): ")
possible_actions=["rock", "paper", "scissors"]
computer_action= random.choice(user_action)
print(f"\nYou chose {user_action}, computer chose {computer_action}.\n")
if user_action == computer_action:
    print(f"Both players selected {user_action}. It's a tie!")
elif user_action == "rock":
    if computer_action == "scissors":
        print("Rock smashes scissors! You win!")
    else:
        print("Paper covers rock! You lose.")
elif user_action == "paper":
    if computer_action == "rock":
        print("Paper covers rock! You win!")
    else:
        print("Scissors cuts paper! You lose.")
elif user_action == "scissors":
    if computer_action == "paper":
        print("Scissors cuts paper! You win!")
    else:
        print("Rock smashes scissors! You lose.")




© 2021 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
Loading complete

