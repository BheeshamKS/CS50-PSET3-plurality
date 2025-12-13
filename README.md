# CS50 PROBLEM SET 3 - Plurality

This repository contains my solution for the Plurality problem from Harvard's CS50 Problem Set 3. The program simulates a simple plurality election where voters cast votes for candidates, and the candidate(s) with the highest number of votes win.

## Files

- `plurality.c` : Main solution file that manages candidates, records votes, and prints the winner(s).

## Description

The program takes candidate names as command-line arguments and then prompts the user to enter votes. It:

- Stores candidates using a struct containing name and vote count
- Validates each vote against the list of candidates
- Tallies votes for valid candidates
- Determines the highest vote count
- Prints the name(s) of the candidate(s) with the most votes
- If multiple candidates are tied for the highest number of votes, all tied candidates are printed.

## Output Behavior

- Invalid votes are rejected and reported
- One or more winners may be printed, depending on ties

## Example Run
```bash
$ ./plurality Alice Bob Charlie
Number of voters: 5
Vote: Alice
Vote: Bob
Vote: Alice
Vote: Charlie
Vote: Alice
Alice
```

How to Run

Compile and run using GCC with the CS50 library:
```bash
gcc -o plurality plurality.c -lcs50
./plurality Alice Bob Charlie
```

Enter each vote when prompted.
