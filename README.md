### form2
---
https://github.com/hughsk/from2

```js
stream = from2([opts], read)

var from = require('from2')
function fromString(string){
  return from(function(size, next){
    if(string.length <= 0) return next(null, null)
    var chunk = string.slice(0, size)
    string = string.slice(size)
    next(null, chunk)
  })
}
fromString('hello world').pipe(process.stdout)
```

```
```

```
```


