# </ C# >

## Thing to Know..
- Case sensitive , use {} for code blocks and ; to end lines.
- Best IDE to use -> visual studio , JetBrains Rider
- Mostly used with .NET framework(Windows-based applications) or .NET core(cross-platform, open-source framework cloud based applications)
- ? operater used to allow value types to be nullable
- Most syntaxas are similar to C,C++ and Java

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

```

## Methods
```bash
int Add(int x, int y)
{
    return x + y;
}

// Method invocation
int result = Add(3, 4); // result = 7

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

```

## 
