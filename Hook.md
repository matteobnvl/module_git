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

```