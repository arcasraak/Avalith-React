# Clase 12 * Viernes 29 de Julio

---

## Funciones y métodos (continuación)

-> El **reduce** lo veremos más adelante

- **1** Métodos más modernos para manipulación de arrays

### Filter

Nos permite iterar por cada elemento de un determinado array y nos devolerá otro array con la información que se corresponda con la condición que le indiquemos en el callback de la función.

Se le pasa un callback (una función que recibe como parámetro otra función)

```
Shapes = [ /, X, /]
Shapes.filter(shape => shape ==/)
[/, /]
```

```
Shapes = [ /, X, /]
Shapes.filter(shape => shape != /)
[X]
```

## Filter en accion

```JavaScript
const users = {
  {
    id:1,
    userName: "Fabi",
    userLastname: "Tureo"
  },
  {
    id:2,
    userName: "Melina",
    userLastname: "Lencinas"
  },
  {
    id: 3,
    userName: "Guillermo",
    userLastName: "Scharf"
  }.
  {
    id: 4,
    userName: "Emi",
    userLastName: "Salias"
  }
}
```

Quiero obtener los users cuyo ID sea menor que 3

```JavaScript
const userLessThanThree = users.filter((user) => user.id < 3);
console.log("Filtrados", userLessThanThree);
```

Quiero obtener los users cuyo ID sea mayor que users

```JavaScript
const userGreaterThanTwo = users.filter((user) => user.id > 2);
console.log("Filtrados", userGreaterThanTwo);
```

Un problema recurrente cuando solicitamos/nos llega la información desde una API (Application Programming Interface) y el caudal de información es mediano/grande, la performance puede verse afectada por el alto costo de métodos en conjunto (si, se puede) para poder crear un algoritmo de mejor rendimiento (no codigo de "mejor rendimiento")


### find

Similar a  lo que hace Filter y Map, Find recorre un array dado y devuelve la primera coincidencia respecto a una condición  dada. A partir de ese momento deja de recorrer el array.

- **2** Spread Operator & Destructuring


---
