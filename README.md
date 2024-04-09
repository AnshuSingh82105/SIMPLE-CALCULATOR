SIMPLE CALCULATOR
Develop a calculator program that performs basic arithmetic
operations such as addition, subtraction, multiplication, and
division. Allow the user to input two numbers and choose an
operation to perform.


this is task given by codesoft
#include <iostream>

using namespace std;

int main() {
    char operation;
    double num1, num2;

    cout << "Enter first number: ";
    cin >> num1;

    cout << "Enter second number: ";
    cin >> num2;

    cout << "Choose an operation (+, -, *, /): ";
    cin >> operation;

    switch(operation) {
        case '+':
            cout << "Result: " << num1 + num2 << endl;
            break;
        case '-':
            cout << "Result: " << num1 - num2 << endl;
            break;
        case '*':
            cout << "Result: " << num1 * num2 << endl;
            break;
        case '/':
            if(num2 != 0)
                cout << "Result: " << num1 / num2 << endl;
            else
                cout << "Error! Division by zero is not allowed." << endl;
            break;
        default:
            cout << "Invalid operation! Please choose from '+', '-', '*', or '/'." << endl;
            break;
    }

    return 0;
}

This code prompts the user to enter two numbers and choose an operation (+, -, *, or /). 
It then performs the selected operation on the two numbers and displays the result. If the user attempts to divide by zero, it displays an error message.
