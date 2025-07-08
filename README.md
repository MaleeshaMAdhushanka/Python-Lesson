# Module Testing Project

A simple Python project demonstrating module imports, function definitions, and the `__name__ == "__main__"` pattern.

## Project Structure

```
Module-Testing/
├── addition.py          # Module containing mathematical functions
├── main.py             # Main script demonstrating module imports
└── README.md           # Project documentation
```

## Files Description

### `addition.py`
A Python module that contains basic mathematical operations:
- `add_numbers(a, b)`: Returns the sum of two numbers
- `subtract_numbers(a, b)`: Returns the difference between two numbers

The module can also be run as a standalone script, demonstrating the `if __name__ == "__main__":` pattern.

### `main.py`
The main script that demonstrates various ways to import and use functions from the `addition` module:
- Direct function import: `from addition import add_numbers`
- Usage examples with different import patterns (commented out)
- Demonstrates best practices for module imports

## Features

- ✅ Basic arithmetic operations (addition, subtraction)
- ✅ Module import demonstrations
- ✅ Proper use of `__name__ == "__main__"` pattern
- ✅ Clean, documented code structure

## How to Run

### Prerequisites
- Python 3.x installed on your system
- VS Code (optional, for development)

### Running the Main Script
```bash
python main.py
```

### Running the Addition Module Directly
```bash
python addition.py
```

## Expected Output

### When running `main.py`:
```
Sum is: 11
```

### When running `addition.py`:
```
You are running addition.py as the main program
8
```

## Code Examples

### Using the Addition Module
```python
from addition import add_numbers, subtract_numbers

# Addition
result = add_numbers(5, 6)
print("Sum is:", result)  # Output: Sum is: 11

# Subtraction
result = subtract_numbers(30, 20)
print("Difference is:", result)  # Output: Difference is: 10
```

### Different Import Patterns
```python
# Method 1: Import specific functions
from addition import add_numbers, subtract_numbers

# Method 2: Import with alias
import addition as math_ops
result = math_ops.add_numbers(5, 3)

# Method 3: Import all (not recommended)
from addition import *
```

## Learning Objectives

This project demonstrates:

1. **Module Creation**: How to create reusable Python modules
2. **Import Patterns**: Different ways to import functions from modules
3. **Main Guard**: Using `if __name__ == "__main__":` to make modules executable
4. **Code Organization**: Separating functionality into logical modules
5. **Best Practices**: Avoiding wildcard imports and naming conventions

## Best Practices Demonstrated

- ✅ Use specific imports instead of `import *`
- ✅ Use descriptive function names
- ✅ Include the main guard pattern
- ✅ Separate concerns into different modules
- ✅ Use aliases for commonly used modules

## Common Import Anti-patterns (Avoided)

```python
# Avoid this - can lead to namespace pollution
from addition import *

# Prefer this - explicit and clear
from addition import add_numbers, subtract_numbers
```

## Future Enhancements

- [ ] Add more mathematical operations (multiplication, division)
- [ ] Add input validation and error handling
- [ ] Include unit tests
- [ ] Add documentation strings (docstrings)
- [ ] Implement a calculator class

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test your changes
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

---

**Note**: This is an educational project designed to demonstrate Python module concepts and import patterns.
