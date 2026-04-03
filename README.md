# Guess-Game-with-3-chances
My 4th Python project - number guess Game 
import random

secret = random.randint(1, 10)
chances = 3

while chances > 0:
    guess = int(input("1 theke 10 er moddhe number guess koro: "))

    if guess == secret:
        print("Wow! Tumi thik guess korecho 🎉")
        break
    else:
        chances = chances - 1
        if chances > 0:
            print("Wrong guess! Aro", chances, "chance ache.")
        else:
            print("Game Over 😢")
            print("Correct number chilo:", secret)
