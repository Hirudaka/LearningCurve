# </ JavaScript >

## Things to Know
-

## Simple Class Constructor

```bash
<!DOCTYPE html>
<html>
<body>
<script>
//What is this? In JavaScript, the this keyword refers to an object. 
//Which object depends on how this is being invoked (used or called). 
//The this keyword refers to different objects depending on how it is used: 
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
