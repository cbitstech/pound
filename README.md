###Pound.js is a small javascript library for storing js objects in browser localStorage.

####Pound.js depends on Underscore.js

###Pound.js API

You can substitute 'p' for 'pound' for the sake of brevity in all pound functions

_To view a list of keys in storage:_
```javascript
pound.list()
//["key1", "key2", "key3"]
```

_To save or update an object:_

```pound.save("[key]", [object])```

_To destroy and object:_

```pound.delete("[key]", [object.id])```

_To return a collection or a single object:_

```pound.find("[key]", options=[{key:value}])```

example:
```javascript
pound.find("cars")
// [{object1}, {object2}, {object3}]
```
```javascript
pound.find("cars", {name: "Camaro"})
// {object2}
```
