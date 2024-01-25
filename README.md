# Author: Michelle Frugia
# GitHub username: frugiam
# Date: 01/24/2024
# Description: Project 3c

target = int(input("Enter the integer for the player to guess.\n"))
guess = int(input("Enter your guess.\n"))
num_guesses = 1
while guess != target:
    if guess > target:
        print("Too high - try again:")
    else:
        print("Too low - try again:")
    guess = int(input(""))
    num_guesses += 1
if num_guesses == 1:
    print("You guessed it in 1 try.")
else:
    print("You guessed it in", num_guesses, "tries.")
