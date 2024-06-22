# bash-file-class6
scripts
# !/bin/bash

# Define the target number
target_number=7

# Initialize the user_guess variable
user_guess=0

# Loop until the user guesses the correct number
until [ $user_guess -eq $target_number ]; do
    # Prompt the user to enter a guess
    echo "Guess the number (between 1 and 10):"
    read user_guess

    # Check if the guess is correct
    if [ $user_guess -eq $target_number ]; then
        echo "Congratulations! You guessed the correct number."
    else
        echo "Incorrect guess. Try again."
    fi
done
