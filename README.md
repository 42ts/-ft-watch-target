# Util - `watchTarget`

get notified when the watch target value changes

## Usage

```javascript
const a = watchTarget('a');

const cleanup = a.watch((a) => console.log(`a is now '${a}'`));
// console output: a is now 'a'

a.get(); // 'a'

a.set('A');
// console output: a is now 'A'

cleanup();

a.set('X'); // (no more console output)
```
