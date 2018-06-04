## Deep Copy

#### =
```javascript (copy reference)
    this.currentModel = this.selectedModel;
```
#### Object.assign (Shallow copy)
```javascript
    this.currentModel = Object.assign({}, this.selectedModel);
```

#### _.clone (Shallow copy)
```javascript
    this.currentModel = _.clone(this.selectedModel);
```

#### stringfy and parse the object (deep copy)
```javascript
    this.currentModel = JSON.parse(JSON.stringify(this.selectedModel));
```


