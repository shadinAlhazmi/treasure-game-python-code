# treasure-game-python-code
print('''
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/_____ /
*******************************************************************************
''')
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.") 


#Write your code below this line 👇
choice1 = input("you\'re at a cross road. where do u want to go? Type 'left' or 'right'. \n").lower()
if choice1 == 'right':
  print("you fell into a hole. Game Over.")
  end_of_game = True

elif choice1 == 'left':
  choice2 = input("you\'ve come to a lake. Type 'swim' to swim across or 'wait' to wait for a boat. \n").lower()

  if choice2 == 'swim':
   print("attacked by trout. Game Over.")
   end_of_game = True

  elif choice2 == 'wait':
    end_of_game = False
    choice3 = input("you\'ve reached the island unharmed. there are 3 doors choose one. red, blue, yellow.\n").lower()
    if choice3 == "red":
      print("u got burned by fire. Game Over.")
    elif choice3 == 'blue':
      print("you got eaten by beasts. Game Over.")
    elif choice3 == 'yellow':
      print("You found the treasure! You Win! 🥳")
    else:
      print("u choose a door that doesn't exist💀- Game Over lol")
