---
difficulty:
  - newbie
OAs:
  - strings
projects:
  - cipher
  - card validation
---

# middleThree

[https://the-winter.github.io/codingjs/exercise.html?name=middleThree&title=String-1](https://the-winter.github.io/codingjs/exercise.html?name=middleThree&title=String-1)

Dada una cadena de longitud impar, devuelva una cadena de longitud 3
desde su centro, por lo que "Candy" produce "and". La longitud de la
cadena será de al menos 3.

__Ejemplo__

```js
    middleThree('Candy') → "and"
    middleThree('and') → "and"
    middleThree('solving') → "lvi"
```
__Solución__
```js
function middleThree(str){
  const strArr = str.split("")
  const middle = Math.trunc(strArr.length/2)
  return `${strArr[middle-1]}${strArr[middle]}${strArr[middle+1]}` 
}
```
