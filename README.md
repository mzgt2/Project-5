# Day-5-Project

# Password Generator

A command-line random password generator that creates secure passwords with customizable length and character types.

## About

Built this to practice working with lists, the random module, and loops in Python. You specify how many letters, symbols, and numbers you want, and it generates a shuffled random password.

## How to Use

Run the program:
```bash
python password_generator.py
```

Answer the prompts:
- How many letters?
- How many symbols?
- How many numbers?

The program generates and displays your random password.

## Example
```
Welcome to the PyPassword Generator!
How many letters would you like in your password?
> 8
How many symbols would you like?
> 2
How many numbers would you like?
> 2

Your password: aK9d#mT2p$Xw
```

(Password will be different each time due to randomization)

## How It Works

1. Get user input for desired password length and composition
2. Use `random.choices()` to select random characters from each category:
   - Letters (lowercase and uppercase)
   - Symbols (!#$%&()*+)
   - Numbers (0-9)
3. Combine all selected characters into one list
4. Shuffle the list using `random.shuffle()` for better security
5. Print each character without spaces using `print(item, end='')`

## Character Sets

**Letters:** a-z, A-Z (52 options)  
**Symbols:** ! # $ % & ( ) * + (9 options)  
**Numbers:** 0-9 (10 options)

## What I Learned

- Using `random.choices(list, k=n)` to select multiple random items
- Converting user input to integers with `int(input())`
- Concatenating lists with the `+` operator
- Shuffling lists in-place with `random.shuffle()`
- Using `for` loops to iterate through lists
- Controlling print output with `end=''` parameter

## Security Features

- Truly random character selection
- Shuffled output (not predictable letter-symbol-number pattern)
- Supports mixed case letters
- Customizable length and composition

## Potential Improvements

If I expand this later:
- Add input validation (ensure positive integers)
- Include more symbol options
- Add password strength indicator
- Option to exclude ambiguous characters (0, O, l, 1)
- Copy password to clipboard automatically
- Save generated passwords to a file (encrypted)
- Add option to generate multiple passwords at once

---

*Learning project - practicing Python lists, random module, and loops*
