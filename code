#include <stdio.h>
#include <stdlib.h>
#include <string.h>

#define MAX_CANDIDATES 10

// Candidate structure
typedef struct {
    char name[50];
    int votes;
} Candidate;

// Function to initialize candidates
void initializeCandidates(Candidate candidates[], int numCandidates) {
    for (int i = 0; i < numCandidates; i++) {
        candidates[i].votes = 0;
    }
}

// Function to display candidates
void displayCandidates(Candidate candidates[], int numCandidates) {
    printf("Candidates:\n");
    for (int i = 0; i < numCandidates; i++) {
        printf("%d. %s\n", i + 1, candidates[i].name);
    }
}

// Function to vote for a candidate
void vote(Candidate candidates[], int candidateIndex) {
    candidates[candidateIndex].votes++;
    printf("You have voted for %s.\n", candidates[candidateIndex].name);
}

// Function to display voting results
void displayResults(Candidate candidates[], int numCandidates) {
    printf("\nVoting Results:\n");
    for (int i = 0; i < numCandidates; i++) {
        printf("%s: %d votes\n", candidates[i].name, candidates[i].votes);
    }
}

int main() {
    int numCandidates;
    printf("Enter the number of candidates: ");
    scanf("%d", &numCandidates);
    
    // Validate the number of candidates
    if (numCandidates <= 0 || numCandidates > MAX_CANDIDATES) {
        printf("Invalid number of candidates.\n");
        return 1;
    }

    Candidate candidates[MAX_CANDIDATES];

    // Initialize candidates
    for (int i = 0; i < numCandidates; i++) {
        printf("Enter the name of candidate %d: ", i + 1);
        scanf("%s", candidates[i].name);
    }

    initializeCandidates(candidates, numCandidates);

    int choice;
    do {
        printf("\nMenu:\n");
        printf("1. Display Candidates\n");
        printf("2. Vote for a Candidate\n");
        printf("3. Display Voting Results\n");
        printf("4. Exit\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);

        switch (choice) {
            case 1:
                displayCandidates(candidates, numCandidates);
                break;
            case 2:
                displayCandidates(candidates, numCandidates);
                printf("Enter the candidate number you want to vote for: ");
                int candidateIndex;
                scanf("%d", &candidateIndex);
                if (candidateIndex < 1 || candidateIndex > numCandidates) {
                    printf("Invalid candidate number.\n");
                } else {
                    vote(candidates, candidateIndex - 1);
                }
                break;
            case 3:
                displayResults(candidates, numCandidates);
                break;
            case 4:
                printf("Exiting...\n");
                break;
            default:
                printf("Invalid choice. Please enter a number between 1 and 4.\n");
        }
    } while (choice != 4);

    return 0;
}
