## Copy Reference: "="
```javascript 
    this.currentModel = this.selectedModel;
```
## Shallow Copy 
#### Object.assign 
An assignment just points a variable at the object that already exists.
```javascript
    this.currentModel = Object.assign({}, this.selectedModel);
```

#### underscore _.clone
_.clone creates a new object and copies each value from the original to the new object.
```javascript
    this.currentModel = _.clone(this.selectedModel);
```

## Deep Copy
#### lodash _.cloneDeep
```javascript
    this.currentModel = _.cloneDeep(this.selectedModel);
```

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


