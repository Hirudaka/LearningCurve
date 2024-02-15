# </ C# >

## Thing to Know..
- C# was developed by Microsoft and first released in 2000 as part of the .NET framework.
- Case sensitive , use {} for code blocks and ; to end lines.
- Best IDE to use -> visual studio , JetBrains Rider
- Mostly used with .NET framework(Windows-based applications) or .NET core(cross-platform, open-source framework cloud based applications)
- ? operater used to allow value types to be nullable
- Most syntaxas are similar to C,C++ and Java
- C# introduced the async and await keywords to simplify asynchronous programming

## Simple Hello World 
```bash
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Hello, world!");
    }
}

```

## Looping Statement

```bash
-- for loop --
for (int i = 0; i < 5; i++)
{
    Console.WriteLine(i);
}

-- while loop --
int j = 0;
while (j < 5)
{
    Console.WriteLine(j);
    j++;
}

-- do-while loop --
int k = 0;
do
{
    Console.WriteLine(k);
    k++;
} while (k < 5);

```
## Exception Handling

```bash
try
{
    int num = int.Parse("abc"); // This will throw FormatException
}
catch (FormatException e)
{
    Console.WriteLine("Invalid format: " + e.Message);
}

```

## Lambda Expressions

```bash
// Lambda expression to calculate square
Func<int, int> square = x => x * x;
int result = square(5); // result = 25

```

## Arrays

```bash
int[] numbers = { 1, 2, 3, 4, 5 };
Console.WriteLine(numbers[0]); // Output: 1

-- multi dimentional arrays --
//Declaration & initialization of a 2D array
int[,] matrix = { { 1, 2, 3 }, { 4, 5, 6 } };

//Accessing elements
int element = matrix[1, 2]; // Accessing element at row 1, column 2 (value: 6)

```

## Methods
```bash
int Add(int x, int y)
{
    return x + y;
}

// Method invocation
int result = Add(3, 4); // result = 7

--overloading methods --
static int PlusMethodInt(int x, int y)
{
  return x + y;
}

static double PlusMethodDouble(double x, double y)
{
  return x + y;
}

static void Main(string[] args)
{
  int myNum1 = PlusMethodInt(8, 5);
  double myNum2 = PlusMethodDouble(4.3, 6.26);
  Console.WriteLine("Int: " + myNum1);
  Console.WriteLine("Double: " + myNum2);
}

```

## Class and Objects 

```bash
class Person
{
    public string Name { get; set; }
    public int Age { get; set; }
}

// Object creation
Person person1 = new Person();
person1.Name = "Alice";
person1.Age = 30;


------ multiple objects ------
class Car
{
  string color = "red";
  static void Main(string[] args)
  {
    Car myObj1 = new Car();
    Car myObj2 = new Car();
    Console.WriteLine(myObj1.color);
    Console.WriteLine(myObj2.color);
  }
}

```

## Math
```bash
// find the highest value of x and y
Math.Max(5, 10);

// find the lowest value of of x and y
Math.Min(5, 10);

//returns the square root of x
Math.Sqrt(64);

//returns the absolute (positive) value of x
Math.Abs(-4.7);

//rounds a number to the nearest whole number
Math.Round(9.99);
```
