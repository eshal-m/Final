# Final
# Algorithm Name: insertion sort
I chose Insertion Sort for ranking applicants because: The dataset is small to medium-sized, and insertion sort is Easy to visualize as it naturally shows how a ranking is built progressively

## Demo video/gif/screenshot of test

Tests:
Missing Values:  Ali, 5.5
<img width="1554" height="880" alt="Screenshot 2026-04-14 142810" src="https://github.com/user-attachments/assets/acd7493e-0e09-4ee0-aa62-3e01ba55d272" />


Invalid GPA:  Ali, 5.5, 50, 80
<img width="1256" height="865" alt="Screenshot 2026-04-14 143526" src="https://github.com/user-attachments/assets/3e4a1dc2-4568-4594-ba95-726194c4a54d" />


Missing Values: Ali, 3.7
<img width="1387" height="878" alt="Screenshot 2026-04-14 143653" src="https://github.com/user-attachments/assets/ff0a2a5b-7e89-416a-859f-f3cde8dde228" />


Empty Input: ()
<img width="934" height="525" alt="Screenshot 2026-04-14 143814" src="https://github.com/user-attachments/assets/527e31ff-4609-4e92-be10-9ddad1c58fc0" />

## Problem Breakdown & Computational Thinking

Key Assumptions:
Each applicant has valid numeric values for:
GPA (0–4)
Volunteer hours (≥ 0)
Essay score (0–100)

Required Preconditions:
Input must follow format:
name, GPA, volunteer_hours, essay_score
GPA must be between 0 and 4
Essay score must be between 0 and 100
Volunteer hours must be non-negative

How the App Enforces This:
The program parses each line individually
It checks:
number of values (must be 4), data types (must be numeric where required), valid ranges
If an error occurs:
The line is ignored
A message is shown to the user explaining the issue

The user sees:
Final Score Explanation
Formula is shown clearly
Explains weighting
Top N Applicants
Clean summary of best candidates
Full Ranking Table
Shows all applicants with scores
Sorting Steps 
During sorting, Each step is described in plain English:

COMPUTATIONAL THINKING CONCEPTS
Decomposition
- Parse input text into structured data
- Compute final score for each applicant
- Loop through applicants (starting from second)
- Compare current applicant with previous ones
- Shift lower-scoring applicants right
- Insert current applicant in correct position
- Repeat until fully sorted


Pattern Recognition

The algorithm repeatedly takes one applicant and compares it to those before it
- Moves lower scores one position right
- Inserts the key in the correct spot
This is the pattern of insertion sort

Abstraction:
Only nessessary inputs are taken from the user. And information that is not important to the ranking is not used in the algorithm. For example, the names of the people do not at all matter in the ranking, so this information is not used in the algorithm and is not focused on. The most important info is gpa, essay, and volunteer hours, so there is no need to focus on anythinng else.

Algorithm Design 
Input:
User enters applicants as text
User selects Top N

Processing:
Validate and parse input
Compute final scores
Apply insertion sort
Record each step of sorting

Output:
Summary of scoring formula
Top N applicants
Full ranked list
Step-by-step simulation

FLOWCHART:
- START
-   ↓
- User inputs applicant data + Top N
-   ↓
- Parse input line by line
-   ↓
- Validate data
-   ↓
- IF invalid → show error message
-   ↓
-   compute final scores
-   ↓
- Apply Insertion Sort:
-    For each applicant:
- Compare with previous
  -     Shift lower scores
-       Insert in correct spot
  ↓
- Generate:
   - Top N list
   - Full ranking
   - Step-by-step explanation
-   ↓
- Display results in GUI
-   ↓
- END
#

## Steps to Run
Enter the name, and variables in the shown format. Then click the button to rank, and the lists will pop up along with explanation. If there are invalid values, the application will display error on those and encourage correcting input format 

## Hugging Face Link
https://huggingface.co/spaces/eshal-m/FinalCISC121

## Author & AI Acknowledgment
I wrote the initial code myself, however I am not much familiar with how to use graphics, so I used ChatGPT to help me write the coding for the visuals. And I also used it to refine my draft code into something smoother, and to better handle all possible edge cases
