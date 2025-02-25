#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;

void problem1() {

    int sum = 0;
    for (int i = 1; i <= 100; i++) {
        sum += i;
    }
    cout << "Sum of first 100 natural numbers: " << sum << endl;

    int n;
    cout << "Enter a positive integer: ";
    cin >> n;

    sum = 0;
    int i = 1;
    while (i <= n) {
        sum += i;
        i++;
    }
    cout << "Sum of first " << n << " natural numbers: " << sum << endl;
}


bool isPrime(int num) {
    if (num <= 1) return false;
    for (int i = 2; i * i <= num; i++) {
        if (num % i == 0) return false;
    }
    return true;
}

void problem2() {

    int count = 0, num = 2;
    cout << "First 10 prime numbers: ";
    while (count < 10) {
        if (isPrime(num)) {
            cout << num << " ";
            count++;
        }
        num++;
    }
    cout << endl;


    int n;
    cout << "Enter the value of n: ";
    cin >> n;

    count = 0, num = 2;
    cout << "First " << n << " prime numbers: ";
    while (count < n) {
        if (isPrime(num)) {
            cout << num << " ";
            count++;
        }
        num++;
    }
    cout << endl;
}


void problem3() {
    int n;
    cout << "Enter a positive integer: ";
    cin >> n;

    cout << "Collatz sequence: " << n << " ";
    while (n != 1) {
        if (n % 2 == 0) {
            n /= 2;
        } else {
            n = 3 * n + 1;
        }
        cout << n << " ";
    }
    cout << endl;
}

void problem4() {
    int num, count = 0;
    cout << "Enter a positive integer: ";
    cin >> num;

    while (num != 0) {
        num /= 10;
        count++;
    }
    cout << "Number of digits: " << count << endl;
}


void problem5() {
    int num;
    cout << "Enter a positive integer: ";
    cin >> num;

    cout << "Digits from right to left: ";
    while (num != 0) {
        cout << num % 10 << " ";
        num /= 10;
    }
    cout << endl;
}


void problem6() {
    int a, b;
    cout << "Enter two positive integers: ";
    cin >> a >> b;

    while (b != 0) {
        int temp = b;
        b = a % b;
        a = temp;
    }
    cout << "GCD: " << a << endl;
}


void problem7() {
    int num, sum = 0, count = 0;

    while (sum <= 100) {
        cout << "Enter a number: ";
        cin >> num;
        sum += num;
        count++;
    }

    cout << "Sum exceeded 100! Total sum: " << sum << endl;
    cout << "Total numbers entered: " << count << endl;
}


void problem8() {
    int balance = 500, withdrawal;

    while (balance > 0) {
        cout << "Your balance: $" << balance << endl;
        cout << "Enter withdrawal amount (or 0 to cancel): ";
        cin >> withdrawal;

        if (withdrawal == 0) break;

        if (withdrawal > balance) {
            cout << "Insufficient funds!" << endl;
        } else {
            balance -= withdrawal;
            cout << "Remaining balance: $" << balance << endl;
        }
    }

    if (balance == 0) {
        cout << "Your balance is now $0. Exiting..." << endl;
    }
}


void problem9() {
    char input;

    do {
        cout << "Enter 'Y' or 'N': ";
        cin >> input;
    } while (input != 'Y' && input != 'N');

    cout << "Accepted" << endl;
}


void problem10() {
    int choice;

    do {
        cout << "ATM Menu:" << endl;
        cout << "1: Withdraw" << endl;
        cout << "2: Deposit" << endl;
        cout << "3: Check Balance" << endl;
        cout << "4: Exit" << endl;
        cout << "Enter your choice: ";
        cin >> choice;

        switch (choice) {
            case 1: cout << "Processing..." << endl; break;
            case 2: cout << "Processing..." << endl; break;
            case 3: cout << "Processing..." << endl; break;
            case 4: cout << "Goodbye!" << endl; break;
            default: cout << "Invalid choice!" << endl;
        }
    } while (choice != 4);
}


void problem11() {
    int choice, a, b;

    do {
        cout << "Menu:" << endl;
        cout << "1: Add" << endl;
        cout << "2: Subtract" << endl;
        cout << "3: Multiply" << endl;
        cout << "4: Exit" << endl;
        cout << "Enter your choice: ";
        cin >> choice;

        if (choice >= 1 && choice <= 3) {
            cout << "Enter two numbers: ";
            cin >> a >> b;
        }

        switch (choice) {
            case 1: cout << a + b << endl; break;
            case 2: cout << a - b << endl; break;
            case 3: cout << a * b << endl; break;
            case 4: cout << "Goodbye!" << endl; break;
            default: cout << "Invalid choice!" << endl;
        }
    } while (choice != 4);
}

void problem12() {
    string password = "1234";
    string input;
    int attempts = 0;

    while (attempts < 3) {
        cout << "Enter password: ";
        cin >> input;

        if (input == password) {
            cout << "Access Granted" << endl;
            break;
        } else {
            cout << "Incorrect" << endl;
            attempts++;
        }
    }

    if (attempts == 3) {
        cout << "Maximum attempts reached!" << endl;
    }
}


void problem13() {
    srand(time(0));
    int secret = rand() % 100 + 1;
    int guess;

    do {
        cout << "Guess: ";
        cin >> guess;

        if (guess < secret) {
            cout << "Too low" << endl;
        } else if (guess > secret) {
            cout << "Too high" << endl;
        } else {
            cout << "Correct!" << endl;
        }
    } while (guess != secret);
}


void welcomeMessage() {
    cout << "Welcome to the C++ programming world!" << endl;
}

void problem14() {
    welcomeMessage();
}


void greetUser() {
    string name;
    cout << "Enter your name: ";
    cin >> name;
    cout << "Hello, " << name << "!" << endl;
}

void problem15() {
    greetUser();
}


int maxNumber(int a, int b) {
    return (a > b) ? a : b;
}

void problem16() {
    int a, b;
    cout << "Enter two numbers: ";
    cin >> a >> b;
    cout << "Maximum: " << maxNumber(a, b) << endl;
}


int factorial(int n) {
    int result = 1;
    for (int i = 1; i <= n; i++) {
        result *= i;
    }
    return result;
}

void problem17() {
    int n;
    cout << "Enter a number: ";
    cin >> n;
    cout << "Factorial: " << factorial(n) << endl;
}


void printRectangle(int width, int height) {
    for (int i = 0; i < height; i++) {
        for (int j = 0; j < width; j++) {
            cout << "*";
        }
        cout << endl;
    }
}

void problem18() {
    int width, height;
    cout << "Enter width and height: ";
    cin >> width >> height;
    printRectangle(width, height);
}


int main() {
    problem1();
    problem2();
    problem3();
    problem4();
    problem5();
    problem6();
    problem7();
    problem8();
    problem9();
    problem10();
    problem11();
    problem12();
    problem13();
    problem14();
    problem15();
    problem16();
    problem17();
    problem18();

    return 0;
}
