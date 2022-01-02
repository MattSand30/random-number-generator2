# random-number-generator2

import random

# Random Numbergenerator Guesser

print("Hello and welcome to the random number guesser.")
print("I am guessing a number of 1 - 20. Can you guess which one?")

x = random.randint(1,20)

# Here you guess the number value of 'x'
for randomNumber in range (1,7):
    randomGuess = input()
    if randomGuess > x:
        print("Too high. Guess again!")
    elif randomGuess < x:
        print("Too low. Guess again!")
    else:
        break

# Checks to see if the number you were guessing is correct or takes you to a fail screen.
if randomGuess == x:
    print("Correct number!")
else:
    print("Too many tries. You have failed. The number I was thinking of was " + (x))``
