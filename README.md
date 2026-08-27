# ECE2112_PA1

**Made by: Montillana,Jasmine Marie P. | 2ECE-B**


This repository contains the completed Programming Assignment 1 for ECE2112. The project covers basic Python string operations, slicing, concatenation, built-in string methods, and extended sequence unpacking without external libraries. 

## A. Word Rotation Problem

Create a function named `rotate_word()` that accpets a non-empty string and moves its first character to the end while keeping all remaining characters in their original order. 

Key functions and methods used in this problem:

Slicing (`text[1:]` and `text[:1]`) : Extracts parts of the string without modifying the original data. `text[1:]` retrieves all characters starting from index 1 to the end, while `text[:1]` extracts the first character.

String Concatenation (`+`): Merges the sliced substring and the isolated first character together.

Below is the complete Python code implementation for this function:
```python
def rotate_word(text):
  return text[1:] + text[:1]
rotate_word('python')
```
## B. Username Builder Problem
Create a function named `make_username()` that accepts two string arguments (first_name and last_name), converts all character to lowercase, removes spaces, and joins them using a perion (.).

Key functions and methods used in this problem:

`.lower()`: A built-in string method that converts all uppercase characters in a string to lowercase. 

String Concatenation (+): Joins the lowercase first name, a dot separator ".", and the lowercase last name.

(Note: If handling names with spaces such as "Jasmine Marie" or "De Jesus", `.replace(" ", "")` can be chained before concatenating.)

Below is the complete Python code implementation for this function:
```python
def make_username(first_name, last_name):
  return first_name.lower() + "." + last_name.lower()
make_username("Jasmine", "Montillana")
```

