</ # JavaScript - Beginner >

## Variables

- **"var**" , **"let**" and **"const"** variables try their behaviors.

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
- Create a class and, define a method inside the class, after that, create an object from the class and execute the methods.
