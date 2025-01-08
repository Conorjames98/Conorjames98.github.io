+++
date = '2024-12-16T12:41:31Z'
draft = false
title = 'Traffic prediction'
+++

# A Traffic prediction program


This application was made to simply predict 
the flow fo traffic at three different 
checkpoints by using an aritmetic sequence 
to calculate the nth term of sequence.


The program starts with an inital starting point for each checkpoint 
and an inital increase for each checkpoint representing the common difference 
and the first term of the sequence. 

The program also asks the user which checkpoint they would like to checkpoint to check and then uses
the formula a1 + (n - 1) * d to calculate the sequence at that checkpoint.


```py
checkpoint_1_start = 12  # First term for checkpoint 1
checkpoint_1_increase = 4  # Common difference for checkpoint 1

checkpoint_2_start = 8   # First term for checkpoint 2
checkpoint_2_increase = 5  # Common difference for checkpoint 2

checkpoint_3_start = 15  # First term for checkpoint 3
checkpoint_3_increase = 2  # Common difference for checkpoint 3

total_minutes = 5  # Term we are calculating up to

# Define a function to calculate the nth term for an arithmetic sequence
def arithmetic_sequence(a1, d, n):
    # Calculate nth term with the formula a1 + (n - 1) * d
    return a1 + (n - 1) * d

# Create a variable for the checkpoint and assign the user's input to it
checkpoint = int(input("Which checkpoint would you like to check? 1, 2, or 3: "))

# If statement to check if the user enters 1
if checkpoint == 1:
    print("This is checkpoint one!")
    for i in range(1, total_minutes + 1):
        cars = arithmetic_sequence(checkpoint_1_start, checkpoint_1_increase, i)
        print(f"At minute {i}: {cars} cars")

# Elif statement to check if the user enters 2
elif checkpoint == 2:
    print("This is checkpoint two!")
    for i in range(1, total_minutes + 1):
        cars = arithmetic_sequence(checkpoint_2_start, checkpoint_2_increase, i)
        print(f"At minute {i}: {cars} cars")

# Elif statement to check if the user enters 3
elif checkpoint == 3:
    print("This is checkpoint three!")
    for i in range(1, total_minutes + 1):
        cars = arithmetic_sequence(checkpoint_3_start, checkpoint_3_increase, i)
        print(f"At minute {i}: {cars} cars")

# Else statement to check if the user enters anything other than 1, 2, or 3
else:
    print("Not in range! Please enter a checkpoint number between 1 and 3.")
    ```









