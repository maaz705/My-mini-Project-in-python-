# Game(rock,paper,scissor)
  
`code`
```python
  import random

item_list: list[str] = ["Rock", "Paper", "Scissor"]
user_choice: str = input("Enter your move (Rock, Paper, Scissor): ")

# Convert user input to title case to match the item_list
user_choice = user_choice.capitalize()

comp_choice = random.choice(item_list)

print(f"user choice = {user_choice}, computer choice = {comp_choice}")

if user_choice == comp_choice:
    print("Both choices are the same = Match tie")

elif user_choice == "Rock":
    if comp_choice == "Paper":
        print("Paper covers Rock = Computer wins")
    else:
        print("Rock smashes Scissor = You win")

elif user_choice == "Paper":
    if comp_choice == "Scissor":
        print("Scissor cuts Paper = Computer wins")
    else:
        print("Paper covers Rock = You win")

elif user_choice == "Scissor":
    if comp_choice == "Paper":
        print("Scissor cuts Paper = You win")
    else:
        print("Rock smashes Scissor = Computer wins")

else:
    print("Invalid choice! Please choose Rock, Paper, or Scissor.")
```

