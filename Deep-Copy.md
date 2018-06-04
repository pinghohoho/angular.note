## copy reference

#### =
```javascript 
    this.currentModel = this.selectedModel;
```
## Shallow copy

#### Object.assign (Shallow copy)
```javascript
    this.currentModel = Object.assign({}, this.selectedModel);
```

#### underscore _.clone
```javascript
    this.currentModel = _.clone(this.selectedModel);
```

## deep copy

#### stringfy and parse the object
will lose properties that are not able to be serialized

```javascript
    var o = {
    a: 1,
    b: 2,
    sum: function() { return a + b; }
};

var o2 = JSON.parse(JSON.stringify(o));
console.log(o2);
```


