## Features

- Customizable password length
- Includes letters (uppercase & lowercase)
- Includes numbers
- Includes symbols
- Randomized order for better security

---

## Installation

1. Make sure you have Python installed (version 3.x recommended).
2. Clone this repository:

```
Navigate to the project folder:

Copy code
cd password-generator
Run the program:

Copy code
python password_generator.py
Usage
Run the program.

Enter the number of letters, numbers, and symbols you want in your password.

The program will generate a randomized password based on your input.

Example:

pgsql
Copy code
Welcome to the password generator
Enter the number of letters in the password: 5
Enter the number of numbers in the password: 3
Enter the number of symbols in the password: 2
Your password is: gT9!a2B#x
Code Example
python
Copy code
import random

letters = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ'
numbers = '0123456789'
symbols = '!@#$%&*'

def password_generator():
    print("Welcome to the password generator")
    n_letters = int(input("Enter the number of letters in the password: "))
    n_numbers = int(input("Enter the number of numbers in the password: "))
    n_symbols = int(input("Enter the number of symbols in the password: "))

    password_list = (
        [random.choice(letters) for _ in range(n_letters)] +
        [random.choice(numbers) for _ in range(n_numbers)] +
        [random.choice(symbols) for _ in range(n_symbols)]
    )

    random.shuffle(password_list)
    password = ''.join(password_list)
    print(f"Your password is: {password}")

password_generator()
Contributing
Contributions are welcome! Please submit a pull request or open an issue for suggestions and improvements.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Author
Ankit Kumar
