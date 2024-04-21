*Mini Voting System*

This is a simple C program that simulates a voting system. It allows the creation of a list of candidates and the ability to vote for them. At the end, the votes are tallied and displayed.

->Features:-
- Initialize candidates with zero votes.
- Display a list of candidates.
- Vote for a candidate.
- Display voting results.

->How to Run:-
To run this program, compile it with a C compiler like gcc and execute the resulting binary.

->Usage:-
- the number of candidates when prompted.
- Use the menu to display candidates, vote, or show results.
- To vote, enter the candidate number.
- To exit the program, choose the ‘Exit’ option from the menu.

->Example Usage:-
This code implements a simple voting system in C. Users can input the number of candidates, their names, vote for a candidate, display candidates, and view the voting results. Below is an example usage scenario:

Input:-
Enter the number of candidates: 3
Enter the name of candidate 1: Alice
Enter the name of candidate 2: Bob
Enter the name of candidate 3: Charlie

Menu:-
Display Candidates
Vote for a Candidate
Display Voting Results
Exit

Choice:-
Display Candidates
Candidates: 
            1. Alice
            2. Bob
            3. Charlie
                             
Choice:-
Vote for a Candidate
Enter the candidate number you want to vote for: 2
You have voted for Bob.
Choice:

Display Voting Results
Voting Results:-
                  Alice: 0 votes
                  Bob: 1 votes
                  Charlie: 0 votes
Repeat steps 2-5 until choosing to exit.

This example demonstrates the functionality of the voting system, allowing users to interactively vote for candidates and view the results.

->Main Function Explanation:-
                            The main() function is the entry point of the program. It prompts the user to input the number of candidates and their names, then initializes a list of candidates accordingly. It presents a menu with options to display candidates, vote for a candidate, display voting results, or exit the program. The user's choice is processed using a switch statement, invoking corresponding functions based on the chosen option. The menu is displayed repeatedly until the user chooses to exit.
