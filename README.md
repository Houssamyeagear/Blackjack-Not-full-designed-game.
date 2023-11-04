# Blackjack-Not-full-designed-game.
# im houssam elmahfoudi 13 moroccan i designed this.
import random

answer1 = input("Hello, would you like to play some blackjack?\n")
if answer1.lower() == "yes":
    print("Roll a dice. You have to keep getting numbers until you reach 21. If you fail, you'll have one chance against the house.\n")
    roll1 = random.randint(1, 10)
    print(str(roll1) + " This is your first roll. Keep rolling until you reach 21.\n")
    roll2 = random.randint(1, 10)
    print(str(roll2) + " 2nd reroll you still cannot stick.\n")
    roll3 = roll1 + roll2 + random.randint(1, 10)
    print(str(roll3) + " Your rolls are done, and now you are forced to stick.\n")
    answer = input("Do you want to stick or continue?\n")
    if roll1 + roll2 == 21:
        print("You won blud.")
    elif roll1 + roll2 + roll3 == 21:
        print("You won bruh :/")
    elif answer.lower() == "stick":
        print("Now I'll roll for the house.\n")
        rollhouse1 = random.randint(1, 10)
        print(str(rollhouse1) + " second roll for house hehe,be ready to lose :D.\n")
        rollhouse2 = rollhouse1 + random.randint(1, 10)
        if rollhouse2 < roll3:
            print("You lost (you have a higher number than the house)well your luck suck :skull:")
        elif rollhouse2 > roll3:
            print("You won(you have a lower number than the house ) nice luck .")
    else:
        print("blud didn't i told you to fkin type stick?")
else:
    print("then get out of this.")



# execute this with python compiler or sum shit its ur choice.
