# BigInt Implementation in C++

This project provides an implementation of arbitrary-precision integers (**BigInt**) in C++ using `std::string` to handle numbers of virtually unlimited size. It supports basic arithmetic operations and comparisons similar to built-in integer types.

## 🚀 Features

- **Arbitrary-length integer storage**
- **Support for positive and negative numbers**
- **Arithmetic operations:**
  - Addition
  - Subtraction
  - Multiplication
  - Division (optional or limited precision)
- **Relational operations:**
  - Equal to, Not equal to
  - Greater than, Less than
  - Greater than or equal to, Less than or equal to
- **Input and output via `cin` / `cout`**

## 📁 Project Structure
```
BigInt/
├── BigInt.h # Header file for BigInt class
├── BigInt.cpp # Implementation of BigInt class
├── main.cpp # Sample usage and test cases
├── README.md # Project documentation
```
## 🧠 How It Works

- **Internal Representation**: Large integers are stored as strings, with digits in reverse for easy calculation (least significant digit first).
- **Sign Handling**: A `bool isNegative` or sign character is used to handle negative numbers.
- **Arithmetic Algorithms**: Mimics the way we do math by hand (grade-school algorithms).

## 🛠️ Usage

### Include the Header

```cpp
#include "BigInt.h"
```
###Example
```
#include <iostream>
#include "BigInt.h"

int main() {
    BigInt num1("123456789012345678901234567890");
    BigInt num2("987654321098765432109876543210");

    BigInt sum = num1 + num2;
    std::cout << "Sum: " << sum << std::endl;

    BigInt product = num1 * num2;
    std::cout << "Product: " << product << std::endl;

    return 0;
}
```
