# </ JavaScript - Beginner >

Written By - Hirudaka Kumarasinghe

## Variables

- **"var**" , **"let**" and **"const"** variables try their behaviors.
- ```var``` was the original way to declare variables in JavaScript.
- ```const``` are variables that cannot be reassigned.
- Variables declared with ```let``` are accessible only within the ***block {}*** in which they are declared.

```bash
<!DOCTYPE html>
<html>
<body>
<script>
let a = 10;
function f() {
  if (true) {
      let b = 9
  // It prints 9
  console.log(b);
  }
  // It gives error as it
  // defined in if block
  console.log(b);
}
f()
// It prints 10
console.log(a)
</script>
<p>Press F12 and see the result in the console view.</p>
</body>
</html>
```

```bash
<!DOCTYPE html>
<html>
<body>
<script>
const a = {
    prop1: 10,
    prop2: 9
}
// It is allowed
a.prop1 = 3
// It is not allowed
a = {
    b: 10,
    prop2: 9
}
</script>
<p>Press F12 and see the result in the console view.</p>
</body>
</html>
```

## Classes

- The ```this``` keyword refers to an object.
- Which object depends on how this is being invoked (used or called).
- The ```this``` keyword refers to different objects depending on how it is used:

> - Creating a class and, define a method inside the class, after that, create an object from the class and execute the methods.

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

### Class Inheritance

```bash
<!DOCTYPE html>
<html>
<body>
<script>

class Car {
  constructor(name) {
  this.brand = name;
  }
  present() {
  return 'I have a ' + this.brand;
  }
}
class Model extends Car {
  constructor(name, mod) {
    super(name);
    this.model = mod;
  } 
  show() {
    return this.present() + ', it is a ' + this.model
  }
}
const mycar = new Model("Ford", "Mustang");
document.write(mycar.show());

</script>
</body>
</html>
```


