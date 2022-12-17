<b>Merging 2 arrays and remove the duplicates</b>

There is no default implementation of merging and removing the duplicates - so we need to do this by iterating over the 2 arrays. 

```javascript
let array1 = ['a', 'b', 'c', 'd']
let array2 = ['d', 'e']
let array3 = []

array1.forEach((element) => {
    array3.push(element)
})

array2.forEach((element) => {
    if(!array3.includes(element)){
        array3.push(element)
    }
})

console.log(array3)
```
