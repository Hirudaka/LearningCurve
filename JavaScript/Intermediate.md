# </ JavaScript >

### Written By - Hirudaka Kumarasinghe

## Things to Know
- Commonly Known as the programming language of the Web.
- Consistently ranked as one of the most in-demand programming languages in the job market.
- ```JavaScript Object Notation (JSON)``` is a lightweight data interchange format inspired by JavaScript object syntax.
- **Runs Everywhere** - JavaScript is a ```multi-paradigm language``` that can run not only in web browsers but also on servers, mobile devices, IoT devices, and more.
- JavaScript uses ```prototypal inheritance``` rather than ```classical inheritance```. (objects can directly inherit from other objects, allowing for flexible and powerful object-oriented programming)
- Dynamically typed, meaning variable types are determined at runtime rather than compile time. (provides flexibility but can also lead to errors if types are not handled properly)
- JavaScript is essential for creating dynamic web content, such as interactive forms, animations, games, and real-time updates.
- Has a rich ecosystem of libraries and frameworks( React, Angular, and Vue.js for front-end development and Express.js for back-end development)

## Objects
- In JavaScript, an object is a standalone entity, with properties and type.

```bash
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Objects</h2>
<p id="demo"></p>

<script>

// Animal properties and method encapsulation
const Animal = {
    type: "Invertebrates", //Default value of properties
    displayType() {
        // Method that display type of Animal
        console.log(this.type);
    },
};

// Create new animal type called animal1
const animal1 = Object.create(Animal);
animal1.displayType(); // Logs: Invertebrates

// Create new animal type called fish
const fish = Object.create(Animal);
fish.type = "Fishes";
fish.displayType(); // Logs: Fishes

</script>
</body>
```

## Simple Class Constructor

- The ```this``` keyword refers to an object.
- Which object depends on how this is being invoked (used or called).
- The ```this``` keyword refers to different objects depending on how it is used:

```bash
<!DOCTYPE html>
<html>
<body>
<script>

//In an object method, this refers to the object.
class Car {
    constructor(name) {
    this.brand = name;
    }
        present() {
            return 'I have a ' + this.brand;
        }
    }
const mycar = new Car("Ford");
document.write(mycar.present());
</script>
</body>
</html>
```

## Closure

- Closure is a function having access to the parent scope, even after the parent function has closed.
- Closure gives you access to an outer function's scope from an inner function. 

```bash
<!DOCTYPE html>
<html>
<body>
<h2>JavaScript Closure</h2>

<p id="demo"></p>

<script>
function greeting() {
    let message = 'Hello Im Hirudaka';
    function sayHi() {
        console.log(message);  //'hello im hirudaka' output
    }
    return sayHi;
}
let hi = greeting();
hi(); // still can access the message variable'
</script>

</body>
</html>
```

## JSON Placeholder API

- Application programming interface is a way for two or more computer programs to communicate with each other. It is a type of software interface, offering a service to other pieces of software.

```bash
<!DOCTYPE html>
<html>
<body>
    <h2>JSON Placeholder API</h2>
    <p id="demo"></p>

    <script>
    //https://jsonplaceholder.typicode.com/
    //Free fake API for testing and prototyping.
    fetch('https://jsonplaceholder.typicode.com/todos/1')
    .then(response => response.json())
    .then(json => console.log(json))
    </script>

</body>
</html>
```

## Array Methods

```bash
<!DOCTYPE html>
<html>
<body>
    <h1 id="demo"></h1>

<script>
const array1 = [1, 4, 9, 16];

// Pass a function to map
const map1 = array1.map(x => x * 2);

document.getElementById("demo").innerHTML = map1;
// Expected output: Array [2, 8, 18, 32]

</script>

</body>
</html>

```
## Destructing 

### Destruction of a Function Returning an array

```bash
<!DOCTYPE html>
<html>
<body>
<script>
    
function calculate(a, b) {
    const add = a + b;
    const subtract = a - b;
    const multiply = a * b;
    const divide = a / b;
    return [add, subtract, multiply, divide];
}
const [add, subtract, multiply, divide] = calculate(4, 7);
document.write("<p>Sum: " + add + "</p>");
document.write("<p>Difference " + subtract + "</p>");
document.write("<p>Product: " + multiply + "</p>");
document.write("<p>Quotient " + divide + "</p>");

</script>
</body>
</html>
```

### Deeply Nested Object Destruction

```bash
<!DOCTYPE html>
<html>
<body>
<p id="demo"></p>
<script>

const vehicleOne = {
    brand: 'Ford',
    model: 'Mustang',
    type: 'car',
    year: 2021, 
    color: 'red',
    registration: {
        city: 'Houston',
        state: 'Texas',
        country: 'USA'
    }
}

myVehicle(vehicleOne)
function myVehicle({ model, registration: { state } }) {
    const message = 'My ' + model + ' is registered in ' + state + '.';
document.getElementById("demo").innerHTML = message;
}

</script>

</body>
</html>
```
