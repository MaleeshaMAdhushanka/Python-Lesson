# My Calculator Package

A simple Python calculator package that provides basic arithmetic operations.

## Project Structure

```
Package-Test1/
├── main.py                 # Main script demonstrating package usage
├── my_calculator/          # Calculator package directory
│   ├── __init__.py        # Package initialization file
│   ├── addition.py        # Addition functionality
│   └── subtract.py        # Subtraction functionality
└── README.md              # This file
```

## Features

- **Addition**: Add two numbers together
- **Subtraction**: Subtract one number from another
- **Package-based structure**: Clean, modular code organization

## Installation

1. Clone or download this project to your local machine
2. Ensure you have Python 3.x installed on your system
3. Navigate to the project directory

## Usage

### Running the Main Script

```bash
python main.py
```

This will demonstrate the calculator package by performing sample calculations:
- Addition: 5 + 3 = 8
- Subtraction: 10 - 4 = 6

### Using the Package in Your Code

You can import and use the calculator package in different ways:

#### Method 1: Import the entire package
```python
import my_calculator

result1 = my_calculator.add(5, 3)      # Returns 8
result2 = my_calculator.sub(10, 4)     # Returns 6
```

#### Method 2: Import specific functions
```python
from my_calculator import add, sub

result1 = add(5, 3)      # Returns 8
result2 = sub(10, 4)     # Returns 6
```

#### Method 3: Import individual modules
```python
from my_calculator import addition, subtract

result1 = addition.add(5, 3)        # Returns 8
result2 = subtract.sub(10, 4)       # Returns 6
```

## Functions

### Addition
- **Function**: `add(a, b)`
- **Parameters**: 
  - `a` (number): First number
  - `b` (number): Second number
- **Returns**: Sum of a and b

### Subtraction
- **Function**: `sub(a, b)`
- **Parameters**: 
  - `a` (number): Number to subtract from
  - `b` (number): Number to subtract
- **Returns**: Difference of a and b (a - b)

## Requirements

- Python 3.x
- No external dependencies required

## Development

This project demonstrates:
- Python package structure
- Module imports and exports
- Clean code organization
- Basic arithmetic operations

## Example Output

When you run `main.py`, you should see:
```
8
6
```

## Contributing

Feel free to extend this calculator package by adding more mathematical operations such as:
- Multiplication
- Division
- Power operations
- Square root
- And more!

## License

This project is open source and available under the MIT License.
