---
difficulty:
  - beginner
OAs:
  - arrays
projects:
  - cipher
  - card validation
---

# Secret Society

[https://edabit.com/challenge/zQm9YZTTFPhNtYjDr](https://edabit.com/challenge/zQm9YZTTFPhNtYjDr)

Un grupo de amigos ha decidido iniciar una sociedad secreta. El nombre de la
sociedad será la primera letra de cada uno de ellos, ordenados alfabéticamente.

Crear una función que tome una serie de nombres y retorne el nombre de la sociedad
secreta.

__Ejemplos__

```js
societyName(["Adam", "Sarah", "Malcolm"]) ➞ "AMS"
societyName(["Harry", "Newt", "Luna", "Cho"]) ➞ "CHLN"
societyName(["Phoebe", "Chandler", "Rachel", "Ross", "Monica", "Joey"]) ➞ "CJMPRR"
```
__Solución__

```js
function societyName(friends) {
	const firstLetters = friends.map(item=>item.charAt(0))
	return firstLetters.sort().join("").toUpperCase()
}
```
> __Importante__ ❗
>
> El nombre de la sociedad secreta debe ser enteramente en mayúsculas.
