---
difficulty:
  - newbie
OAs:
  - strings
  - conditionals
projects:
  - cipher
  - card validation
---

# comboString

[https://the-winter.github.io/codingjs/exercise.html?name=comboString&title=String-1](https://the-winter.github.io/codingjs/exercise.html?name=comboString&title=String-1)

Implementa la función `comboString` para que reciba dos cadenas, a y b, y
devuelva una cadena de la forma `corta + larga + corta`, con la cadena más
corta en el exterior y la cadena más larga en el interior. Las cadenas no
tendrán la misma longitud, pero pueden estar vacías (longitud 0).

__Ejemplo:__

```js
    comboString('Hello', 'hi') → "hiHellohi"
    comboString('Hi', 'Hello') → "HiHelloHi"
    comboString('aaa', 'b') → "baaab"
```
__Solución:__
```js
function comboString(a, b){
  const firstStr = a.length;
  const secondStr = b.length;
 return (firstStr<secondStr)?`${a}${b}${a}`:`${b}${a}${b}`
}
```
