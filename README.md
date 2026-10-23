# Password Strength Checker

A simple command-line Python program that checks whether a password meets basic strength requirements, including minimum length, numbers, uppercase and lowercase letters, and special characters.

## Features

- Checks that a password contains at least 8 characters.
- Verifies that it includes at least one digit.
- Verifies that it includes at least one uppercase letter.
- Verifies that it includes at least one lowercase letter.
- Checks for a special character from the program’s supported set.
- Displays feedback about which requirement is missing.
- Allows users to check multiple passwords in one session.
- Supports typing `exit` to quit the program.

## Requirements

- Python 3
- Python's built-in `re` module (no additional installation required)

## How to Run

1. Download or clone this repository.
2. Open a terminal in the project folder.
3. Run the script:

```bash
python Password_Strength.py
```

Depending on your system, you may need to use `python3` instead of `python`.

## How to Use

When the program starts, enter a password at the prompt. It will display feedback based on the requirements your password meets.

To stop the program, type:

```text
exit
```

## Password Requirements

The checker looks for the following:

| Requirement | Rule |
|---|---|
| Length | At least 8 characters |
| Digit | At least one number, such as `7` |
| Uppercase | At least one uppercase letter, such as `A` |
| Lowercase | At least one lowercase letter, such as `b` |
| Special character | At least one character from `!@#$%^&*(){}<>.?` |

The program returns a message indicating whether a requirement is missing or all of its checks have passed.

## Concepts Practiced

This project helped me practice:

- Python functions and return values
- Conditional statements
- `while` loops
- User input and output
- Generator expressions and `any()`
- String methods such as `isdigit()`, `isupper()`, and `islower()`
- Regular expressions using Python's `re` module
- The `if __name__ == "__main__":` entry-point pattern

## Important Security Note

This is a beginner learning project that checks a few password composition rules. A password that passes these checks is **not necessarily secure**. The program does not measure password entropy, detect common or compromised passwords, or evaluate whether a password is easy to guess.

The current version uses ordinary `input()`, so entered passwords may be visible on the terminal. **Do not enter real or reused passwords into this learning project.**

## Future Improvements

- Hide password input using Python's `getpass` module.
- Provide a more detailed strength score.
- Check passwords against common-password lists or a trusted compromised-password service.
- Add automated tests for the password-checking function.

## Author

Mehr Hussain

Artificial Intelligence Student | Python Learner

[GitHub](https://github.com/DevelopMehr)
