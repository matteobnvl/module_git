### empecher de commit 

```js 
process.exit(1)
console.log("Il est impossible de commit")
```

### vérifie que le message de commit commence par bonjour

```js
if (!commitMsg.startsWith('bonjour')) {
  console.error('Le message de commit doit commencer par "bonjour"');
  process.exit(1);
} else {
  console.log("\x1b[32mCommit message format is valid.\x1b[0m");
  process.exit(0);
}
```

### vérifie que le nombre de caractère du message est pair

```js
if ((commitMessage.length % 2 - 1) !== 0) {
  console.error('Le nombre de caractères dans votre message de commit doit être pair');
  process.exit(1);
} else {
  console.log("\x1b[32mCommit message format is valid.\x1b[0m");
  process.exit(0);
}
```


### hook qui vérifie que le message de commit commence bien au format “XXX-0000” ou les X sont des lettres et les 0 sont des chiffres

```js

```