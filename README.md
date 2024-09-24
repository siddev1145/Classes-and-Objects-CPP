# Classes-and-Objects-CPP

## Experiment 11

## Aim
To learn about classes and objects.

## Software Used
VS Code

## Theory
### Definition
Object-Oriented Programming (OOP) is a programming paradigm that focuses on "objects."

#### What is a Class?
A class is a blueprint for creating objects. It encapsulates data and functions that operate on that data. For example, consider a class called `Dog`:

```cpp
#include <iostream>
using namespace std;

class Dog {
public:
    string name;
    int age;

    void bark() {
        cout << name << " Woof!" << endl;
    }
};
```

#### What is an Object?
An object is an instance of a class. It contains both data (attributes) and methods (functions). For instance, a specific car object might have attributes like color and model and methods like starting the engine or driving.

An object has two main features:
1. **Attributes:** Characteristics of the object, such as color or model for a car.
2. **Methods:** Actions the object can perform, like `start_engine()` or `drive()`.

For example, creating an object of the `Dog` class:

```cpp
int main() {
    Dog myDog;
    myDog.name = "Buddy";
    myDog.age = 3;

    myDog.bark();

    return 0;
}
```

### Principles of OOP in C++

#### 1. Encapsulation
Encapsulation bundles data and methods within a class, hiding the object's internal state and exposing a controlled interface. In C++, this is often achieved by using private or protected data members and public methods (getters and setters).

#### 2. Inheritance
Inheritance allows a derived class to inherit properties and methods from a base class, promoting code reusability. For example:

```cpp
class Animal {
public:
    void eat() { std::cout << "Eating..." << std::endl; }
};

class Dog : public Animal {
public:
    void bark() { std::cout << "Barking..." << std::endl; }
};
```

#### 3. Polymorphism
Polymorphism enables objects of different classes to be treated as objects of a common base class. This allows methods of derived classes to be called through base class pointers or references.

#### 4. Abstraction
Abstraction hides complex implementation details and shows only essential features of an object, simplifying interactions.

## Algorithms
### Define Method Inside Class
1. **Start**
2. **Define the `Student` Class**
   - **Public Section**
     - Define the `myMethod` function to print "I am studying in 2nd year."
3. **Main Function**
   - Create an object `s1` of type `Student`.
   - Call `myMethod` on `s1`.
4. **End**

### Define Method Outside Class
1. **Start**
2. **Define the `Student` Class**
   - **Public Section**
     - Declare the `myMethod` function.
3. **Define `myMethod` Outside the Class**
   - Print "A Sophomore in SIT."
4. **Main Function**
   - Create an object `s1` of type `Student`.
   - Call `myMethod` on `s1`.
5. **End**

### Cuboid Volume Calculation
1. **Start**
2. **Define `Cuboid` Class**
   - **Public Section**
     - Data members: `int length, breadth, height, volume;`
     - Member functions:
       - `input()`: Get dimensions from the user.
       - `Volume()`: Calculate volume using `volume = length * breadth * height`.
       - `Output()`: Print the volume.
3. **Main Function**
   - Create an object `v1` of type `Cuboid`.
   - Call `input()` for `v1`.
   - Call `Volume()` for `v1`.
   - Call `Output()` for `v1`.
4. **End**

## Conclusion
We explored the concepts of classes and objects in OOP.