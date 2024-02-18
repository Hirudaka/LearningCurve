# </ C++ >

## Thing to Know..
>- C++ developed as an extention to C language in 1985
>- Introduced the concept of ```classes and objects```, ```inheritance```, ```encapsulation```, and ```polymorphism```
>- Difference between C and C++ is C++ **support** classes and objects, while C **does not**.
>- Widely used in the game development industry
>- C++ provides mechanisms for dynamic memory allocation and deallocation using **new** and **delete** operators (Unlike Java,C#,Python,Ruby,Javacript)
>- C++11 introduced smart pointers ```(Ex- std::unique_ptr, std::shared_ptr, and std::weak_ptr)```, which help manage **dynamic memory allocation**


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

## Pointers
- Pointers are variables that store memory addresses. They are denoted by "*"

```Deferencing Pointers```
-Dereferencing a pointer means accessing the value stored at the memory address it points to.
-You use the dereference operator * to access the value

```bash
------------Declaring a Pointer----------
int* ptr = &num;

------------Initializing a pointer----------
int num = 10;
int* ptr = &num;

------------Deferencing Pointers------------
int num = 10;
int* ptr = &num;
cout << *ptr; // Prints value stored at the memory address pointed to by ptr (Ex- prints 10)
```
