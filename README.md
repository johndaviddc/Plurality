# Plurality Voting System

This program implements a plurality voting system. The user enters the names of the candidates, then enters the number of voters and their votes. The candidate with the most votes wins.

## Usage
To run the program, open the terminal and navigate to the directory containing the program file. Then compile the program by entering **`make plurality`** in the terminal. Finally, run the program by entering **`./plurality`** followed by the names of the candidates.

For example, to run the program with three candidates named Alice, Bob, and Charlie, enter the following in the terminal:
```sh
./plurality Alice Bob Charlie
```

The program will then prompt the user for the number of voters and their votes.

# How it works
The program first checks that the user has provided at least one candidate name as a command-line argument. It then prompts the user for the number of voters. For each voter, the user enters the name of the candidate they are voting for.

The program keeps track of the vote counts for each candidate using an array of candidate structs. The **`vote`** function updates the vote count for the candidate whose name matches the user's input. The **`print_winner`** function then prints the names of the candidate(s) with the most votes.