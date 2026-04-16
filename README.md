# Final
# Algorithm Name: insertion sort
I chose Insertion Sort for ranking applicants because: The dataset is small to medium-sized, and insertion sort is Easy to visualize as it naturally shows how a ranking is built progressively

## Demo video/gif/screenshot of test

Tests:
Missing Values:  Ali, 5.5
<img width="1235" height="417" alt="Screenshot 2026-04-15 224255" src="https://github.com/user-attachments/assets/380afb36-4e1a-4206-bba5-828a866a7b1e" />


Invalid value (GPA):  Ali, 5.5, 50, 80
<img width="1326" height="505" alt="Screenshot 2026-04-15 224744" src="https://github.com/user-attachments/assets/b169bd7b-83d3-4137-a7a7-02bedb347d15" />


Empty Input: ()
<img width="1216" height="485" alt="Screenshot 2026-04-15 224849" src="https://github.com/user-attachments/assets/b8fde2f6-7f5c-42b2-a430-c7409bd11d59" />


## Problem Breakdown & Computational Thinking
Key Assumptions:
Each applicant has valid numeric values for:
GPA (0–4)
Volunteer hours (≥ 0)
Essay score (0–100)

Required Preconditions:
Input must follow format: name, GPA, volunteer_hours, essay_score
- GPA must be between 0 and 4
- Essay score must be between 0 and 100
- Volunteer hours must be non-negative
- Each applicant name must be unique


How the App Enforces This:
The program parses each line individually and splits input into components, removes extra spaces, and checks, Number of values (must be 4), data types (must be numeric where required), valid ranges, duplicate names
If an error occurs the process stops and a clear error message is displayed to the user

 What the User Sees
Final Ranking List
Swapped or compared elements are highlighted to make movement clear


COMPUTATIONAL THINKING CONCEPTS
Decomposition

The problem is broken into smaller steps:
- Parse input text into structured applicant data
- Compute final score for each applicant
- Apply QuickSort:
- Select a pivot
- Compare elements to the pivot
- Swap elements into correct partitions
- Recursively sort sublists
- Update the displayed list after each swap

Pattern Recognition
The algorithm repeatedly:
- Selects a pivot element
- Compares each item to the pivot
- Moves higher scores to one side and lower scores to the other
This pattern makes up quicksort

Abstraction
Only necessary inputs are used:
GPA
Volunteer hours
Essay score
These are combined into a single final score, which is the only value used for sorting.
Other details (like names) are not used in calculations and only used for display purposes

This simplifies the problem and focuses only on what affects ranking.

## Algorithm Design
Input:name, gpa, hours, essay
Processing:
Validate and parse input
Compute final score using weighted formula
Choose a pivot
Compare elements
Swap elements when needed
Recursively sort subarrays
After each swap, update the displayed list
Output:
- A ranked list
- Applicants visually move into correct positions
- Final sorted list (highest score → lowest score)

## FLOWCHART 
- START
- ↓
- User inputs applicant data
- ↓
- Parse input line by line
- ↓
- Validate data
- ↓
- IF invalid → show error message
- ↓
- Compute final scores
- ↓
- Apply QuickSort:
- Select pivot
- Compare elements to pivot
- Swap elements as needed
- Recursively sort partitions
- ↓
-  Continuously update displayed list during sorting
- ↓
 - Final sorted ranking displayed
- ↓
- END

## Steps to Run
Enter applicants in the format:

name,gpa,hours,essay

Example:

Alice,3.8,120,85
Bob,3.5,200,90
Run the program
The application will:
- Validate the input
- Display the list
- Visually reorder applicants as sorting occurs
If there are invalid values:
The program will display an error message

## Hugging Face Link
https://huggingface.co/spaces/eshal-m/FinalCISC121

## Author & AI Acknowledgment
I wrote the initial code myself, however I am not much familiar with how to use graphics, so I used ChatGPT to help me write the coding for the visuals. And I also used it to refine my draft code into something smoother, and to better handle all possible edge cases
