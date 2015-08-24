## How test case description is formed?

Fully qualified description of a test case is concatenated from partial descriptions from `describe`, `context` and `it` statements.

```js
describe('Array', function () {
  describe('#indexOf', function () {
    it('should return index of passed item', function () {
      // ...
    });
  });
});

describe('/books resource', function () {
  context('when there is no books', function () {
    it('should respond with 200 status code', function () {
      // ...
    });
    
    it('should respond with empty array', function () {
      // ...
    })
  });
});

// Would result in three test cases described as:
//
// Array #indexOf should return index of passed item
// /books resource when there is no books should respond with 200 status code
// /books resource when there is no books should respond with an empty array
```

## Used technologies

* mocha
