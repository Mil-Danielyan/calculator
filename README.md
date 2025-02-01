# calculator
#include <iostream>

int main() {
    double a, b;  

    std::cout << "Enter first number";
    std::cin >> a;
    std::cout << "Enter second number";
    std::cin >> b;
    std::cout << "Enter operation simbol (+, -, *, /): ";
    std::cin >> c;

    if (c == '-') {
        std::cout << "a = " << a - b << "\n";
    } else if (c == '+') {
        std::cout << "b = " << a + b << "\n";
    } else if (c == '*') {
        std::cout << "b = " << a * b << "\n";
    } else if (c == '/') {
        if (b != 0) {
            std::cout << "b = " << a / b << "\n";
        } else {
            std::cout << "ERROR: division by zero is not allowed \n";
        }
    } else {
        std::cout << "ERROR: please enter character +, -, * or / \n";
    }

    switch (c) {
        case '-':
            std::cout << "a = " << a - b << "\n";
            break;
        case '+':
            std::cout << "a = " << a + b << "\n";
            break;
        case '*':
            std::cout << "a = " << a * b << "\n";
            break;
        case '/':
            if (b != 0) {
                std::cout << "a = " << a / b << "\n";
            } else {
                std::cout << "ERROR: division by zero is not allowed\n";
            }
            break;
        default:
            std::cout << "ERROR: please enter character +, -, * կամ / \n";
    }

    return 0;
}
