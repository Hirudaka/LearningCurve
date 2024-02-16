# </ C++ >

## Thing to Know..
- C++ developed as an extention to C language in 1985
- Introduced the concept of ```classes and objects```, ```inheritance```, ```encapsulation```, and ```polymorphism```
- Difference between C and C++ is C++ **support** classes and objects, while C **does not**.
- Widely used in the game development industry
- C++ provides mechanisms for dynamic memory allocation and deallocation using **new** and **delete** operators (Unlike Java,C#,Python,Ruby,Javacript)
- C++11 introduced smart pointers ```(Ex- std::unique_ptr, std::shared_ptr, and std::weak_ptr)```, which help manage **dynamic memory allocation**


## Simple Hello World in C++
```bash
#include <iostream>

int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}
```

## User input strings
```bash
string firstName;
cout << "Type your first name: ";
cin >> firstName; // get user input from the keyboard
cout << "Your name is: " << firstName;
```
