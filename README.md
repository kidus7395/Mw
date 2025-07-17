Absolutely! Below is the full working C++ program that uses cin to enter two numbers and any one of the five arithmetic operators:

✅ Supported operators: +, -, *, /, %
✅ Functions used: add, subtract, multiply, divide, remainder
✅ Handles division by zero safely


---

✅ Updated Full C++ Code:

#include <iostream>
using namespace std;

// Addition function
int add(int a, int b) {
    return a + b;
}

// Subtraction function
int subtract(int a, int b) {
    return a - b;
}

// Multiplication function
int multiply(int a, int b) {
    return a * b;
}

// Division function
float divide(int a, int b) {
    if (b == 0) {
        cout << "Error: Division by zero!" << endl;
        return 0;
    }
    return (float)a / b;
}

// Remainder function
int remainder(int a, int b) {
    if (b == 0) {
        cout << "Error: Division by zero!" << endl;
        return 0;
    }
    return a % b;
}

int main() {
    int x, y;
    char op;

    // User input
    cout << "Enter first number: ";
    cin >> x;

    cout << "Enter operator (+, -, *, /, %): ";
    cin >> op;

    cout << "Enter second number: ";
    cin >> y;

    // Operator handling using switch
    switch(op) {
        case '+':
            cout << "Result: " << add(x, y) << endl;
            break;
        case '-':
            cout << "Result: " << subtract(x, y) << endl;
            break;
        case '*':
            cout << "Result: " << multiply(x, y) << endl;
            break;
        case '/':
            cout << "Result: " << divide(x, y) << endl;
            break;
        case '%':
            cout << "Result: " << remainder(x, y) << endl;
            break;
        default:
            cout << "Invalid operator!" << endl;
    }

    return 0;
}



