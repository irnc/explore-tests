```js
describe('A', () => {
  beforeEach('A beforeEach', () => {
    console.log('A beforeEach');
  });

  it('A it 1', () => {
    console.log('A it 1');
  });

  // Nested contexts should be defined after all `it` cases of a parent.
  context('B', () => {
    before('B before', () => {
      console.log('B before');
    });
    
    // Put `after` right after corresponging `before`.
    after('B after', () => {
    });

    /* `beforeEach` should be placed after `before`.
     * 
     * Because this is the order in which they would be executed.
     */
    beforeEach('B beforeEach', () => {
      console.log('B beforeEach');
    });

    it('B it 1', () => {
      console.log('B it 1');
    });
    
    it('B it 2', () => {
      console.log('B it 1');
    });
  });
});
```
