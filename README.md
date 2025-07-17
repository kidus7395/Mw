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
    int x = 10, y = 3;

    cout << "Addition: " << add(x, y) << endl;
    cout << "Subtraction: " << subtract(x, y) << endl;
    cout << "Multiplication: " << multiply(x, y) << endl;
    cout << "Division: " << divide(x, y) << endl;
    cout << "Remainder: " << remainder(x, y) << endl;

    return 0;
}
