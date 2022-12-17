<b>1. Deep copy vs shallow copy for object </b>

Simple "=" assignment of object will create a deep copy and not a shallow copy. Changing the copied object will also modify the original object. 

```javascript
let t = {
    "name": "Pranav"
}
let b = t
b.name = "Bhatia"
console.log(t)
```
Returns 

```cli
{ name: 'Bhatia' }
```

There are 3 ways to clone an object - 

```javascript
// Spread Method
let clone = { ...userDetails }

// Object.assign() Method
let clone = Object.assign({}, userDetails)

// JSON.parse() Method
let clone = JSON.parse(JSON.stringify(userDetails))
```

