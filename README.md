# NumberGuessingGame.py
A beginner-friendly number guessing game built with Python featuring random number generation, helpful hints, and attempt tracking.
import random

secret_number = random.randint(1, 100)
attempts = 0

print("I'm thinking of a number from 1 to 100.")

while True:
    try:
        guess = int(input("Your guess: "))
    except ValueError:
        print("Please enter a whole number.")
        continue

    if not 1 <= guess <= 100:
        print("Enter a number between 1 and 100.")
        continue

    attempts += 1

    if guess < secret_number:
        print("Too low! Try again.")
    elif guess > secret_number:
        print("Too high! Try again.")
    else:
        print(f"You got it in {attempts} guesses!")
        breakimport random

secret_number = random.randint(1, 100)
attempts = 0

print("I'm thinking of a number from 1 to 100.")

while True:
    try:
        guess = int(input("Your guess: "))
    except ValueError:
        print("Please enter a whole number.")
        continue

    if not 1 <= guess <= 100:
        print("Enter a number between 1 and 100.")
        continue

    attempts += 1

    if guess < secret_number:
        print("Too low! Try again.")
    elif guess > secret_number:
        print("Too high! Try again.")
    else:
        print(f"You got it in {attempts} guesses!")
        break
