# Guess_Game.py
Author - Vaibhav

import random

while True:
    secret_no = random.randint(1, 10)
    attempts = 3

    while attempts > 0:
        user_input = int(input(" Guess the Secret Number: "))

        if user_input == secret_no:
            print("You Guessed it correctly!")
            break
        else:
            attempts -= 1
            print("Guess the Secret Number again" , attempts, "attempts left.")

    else:
        print("The Secret Number is", secret_no)

    play_again = input("Play again? (yes/no): ")
    if play_again != "yes":
        break