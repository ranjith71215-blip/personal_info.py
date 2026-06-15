# Personal Information Program

## Project Overview

### Description
The Personal Information Program is a beginner-friendly Python application that stores personal details and collects user preferences through keyboard input. The program displays the information in a well-formatted layout and performs a simple age calculation.

### Objectives
- Practice using variables in Python
- Learn how to accept user input
- Implement basic input validation
- Use loops for error checking
- Format output using f-strings
- Perform simple calculations

---

## Features

### Static Information
The program stores the following predefined information:

- Name: Ranjith Kumar
- Age: 20
- City: Bangalore
- Hobby: Reading

### Dynamic User Input
The user is prompted to enter:

- Favorite Food
- Favorite Color

### Input Validation
The program ensures that users cannot leave the Favorite Food or Favorite Color fields empty.

### Age Calculation
The program calculates and displays the user's age in months.

Formula:

```python
age_in_months = age * 12
```

### Formatted Output
Information is displayed using headings, separators, and aligned formatting for better readability.

---

## Technologies Used

- Python 3

---

## How to Run the Program

### Prerequisites

Install Python 3 on your computer.

Verify installation:

```bash
python --version
```

or

```bash
python3 --version
```

### Steps

1. Save the program as `personal_info.py`
2. Open Terminal or Command Prompt
3. Navigate to the project folder

```bash
cd project_folder
```

4. Run the program

```bash
python personal_info.py
```

5. Enter your favorite food and favorite color when prompted.

---

## Project Structure

```text
Personal-Information-Program/
│
├── personal_info.py
├── README.md
└── screenshots/
    ├── program_start.png
    ├── user_input.png
    └── output.png
```

---

## Program Flow

```text
Start Program
      │
      ▼
Display Welcome Message
      │
      ▼
Store Personal Information
      │
      ▼
Calculate Age in Months
      │
      ▼
Get Favorite Food
      │
      ▼
Validate Input
      │
      ▼
Get Favorite Color
      │
      ▼
Validate Input
      │
      ▼
Format User Input
      │
      ▼
Display Personal Information
      │
      ▼
End Program
```

---

## Variables Used

| Variable | Type | Description |
|-----------|---------|-------------|
| name | String | User's name |
| age | Integer | User's age |
| city | String | User's city |
| hobby | String | User's hobby |
| age_in_months | Integer | Age converted to months |
| favorite_food | String | User's favorite food |
| favorite_color | String | User's favorite color |

---

## Sample Output

```text
==================================================
WELCOME TO MY PERSONAL INFORMATION PROGRAM
==================================================

Enter your favorite food: Pizza
Enter your favorite color: Blue

==================================================
PERSONAL INFORMATION
==================================================
Name           : Ranjith Kumar
Age            : 20
Age in Months  : 240
City           : Bangalore
Hobby          : Reading
--------------------------------------------------
USER PREFERENCES
--------------------------------------------------
Favorite Food  : Pizza
Favorite Color : Blue
==================================================
Thank you for using the Personal Information Program!
Goodbye!
```

---

## Testing Evidence

### Test Case 1: Valid Input

**Input**

```text
Favorite Food: Pizza
Favorite Color: Blue
```

**Expected Result**

Program displays all information correctly.

**Status:** Passed ✅

---

### Test Case 2: Empty Favorite Food

**Input**

```text
Favorite Food:
```

**Expected Result**

```text
Favorite food cannot be empty. Please try again.
```

**Status:** Passed ✅

---

### Test Case 3: Empty Favorite Color

**Input**

```text
Favorite Color:
```

**Expected Result**

```text
Favorite color cannot be empty. Please try again.
```

**Status:** Passed ✅

---

## Challenges and Solutions

### Challenge 1: Empty User Input

**Problem:**
Users could submit blank responses.

**Solution:**
Implemented `while` loops to repeatedly request input until a valid value is entered.

```python
while favorite_food == "":
    print("Favorite food cannot be empty. Please try again.")
```

---

### Challenge 2: Consistent Formatting

**Problem:**
User-entered text could have inconsistent capitalization.

**Solution:**
Used the `.title()` method to format text.

```python
favorite_food = favorite_food.title()
favorite_color = favorite_color.title()
```

---

### Challenge 3: Displaying Information Clearly

**Problem:**
Output needed to be easy to read.

**Solution:**
Used separators and aligned f-string formatting.

```python
print(f"Name           : {name.title()}")
```

---

## Screenshots

Include the following screenshots:

### Screenshot 1: Program Startup

Shows the welcome screen.

### Screenshot 2: User Input

Shows prompts for favorite food and favorite color.

### Screenshot 3: Final Output

Shows the formatted personal information display.

---

## Future Improvements

Possible future enhancements include:

- Allow users to enter all personal details dynamically
- Store information in a file
- Add menu options
- Support multiple users
- Create a graphical user interface (GUI)
- Connect to a database

---

## Learning Outcomes

Through this project, I learned:

- Variables and data types
- User input and output
- While loops
- Input validation
- String manipulation
- Arithmetic calculations
- Formatted printing using f-strings
- Basic program structure in Python

---

## Conclusion

This project successfully demonstrates fundamental Python programming concepts such as variables, loops, input validation, calculations, and formatted output. It serves as a strong foundation for building more advanced Python applications in the future.
