# remove(dir, callback)

Removes a file or directory. The directory can have contents. Like `rm -rf`.

**Sync:** `removeSync()`

## Example:

```js
const fs = require('fs-extra')

fs.remove('/tmp/myfile', err => {
  if (err) return console.error(err)

  console.log('success!')
})

fs.removeSync('/home/jprichardson') // I just deleted my entire HOME directory.
```
