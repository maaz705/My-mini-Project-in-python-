## Game(rock,paper,scissor)
  
`code`
```python

import random

item_list = ["Rock", "Paper", "Scissor"]

# Commit 1: Initialize variables
user_choice = input("Enter your move (Rock, Paper, Scissor): ")
user_choice = user_choice.capitalize()
comp_choice = random.choice(item_list)

# Commit 2: Display choices
print(f"User choice = {user_choice}, Computer choice = {comp_choice}")

# Commit 3: Handle tie
if user_choice == comp_choice:
    print("Both choices are the same = Match tie")

# Commit 4: Handle Rock
elif user_choice == "Rock":
    if comp_choice == "Paper":
        print("Paper covers Rock = Computer wins")
    else:
        print("Rock smashes Scissor = You win")   


# Commit 5: Handle Paper
elif user_choice == "Paper":
    if comp_choice == "Scissor":
        print("Scissor cuts Paper = Computer wins")
    else:
        print("Paper covers Rock = You win")   


# Commit 6: Handle Scissor
elif user_choice == "Scissor":
    if comp_choice == "Paper":
        print("Scissor cuts Paper = You win")
    else:
        print("Rock smashes Scissor = Computer   
 wins")

# Commit 7: Handle invalid input
else:
    print("Invalid choice! Please choose Rock, Paper, or Scissor.")
```

######
If you need to understand this code and determine what has happened and how it has occurred.


        [to watch this video on youtube ](https://www.youtube.com/watch?v=OvsoAMA_P00&list=PL3JNM3ENFH-5r3mRfuIbXLRCvtNK0FhmU&index=3)
