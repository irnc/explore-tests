# Bad

```js
before(function () {
  // ...
});
```

```
1) Something "before all" hook:
     Error: something went wrong
```

# Good

```js
before(function createUserAccount() {
  // ...
});
```

```
1) Something "before all" hook: createUserAccount:
     Error: something went wrong
```
