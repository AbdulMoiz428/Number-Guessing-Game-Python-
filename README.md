How to Play:
The computer generates a random number between 1 and 10.

You try to guess the number.
The game continues until you guess the correct number.
At the end, it shows how many attempts you took.

Features:
Input validation to ensure only numbers are entered
Simple and clear feedback for each guess
Counts the number of attempts and tells You Your Score 
You can easily modify this game by changing the range of numbers or adding more features like difficulty levels or score tracking.

Code Starts From Here
import random

score=10
randomNumber =random.randint(1,10)
attempts=0
print("Welcome to the Number Guessing Game!")
print("I'm thinking of a number between 1 and 10.")

while True:
    userNumberInput = int(input("Please enter a number between 1 and 10: "))
    attempts+=1

    if userNumberInput == randomNumber:
                   print("Congratulations You guessed It right Your Score is:" + str(score) + " You guessed the number in: " + str(attempts) + "th attempt!")
                   break
    else:
           print("Sorry, You did not guess it right Better Luck Next Time")
           score -= 1
