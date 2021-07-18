# Flat & FlatMap
##### for flattening arrays

```javascript
const animals = [['🐥'], ['🐰'], ['🐷'], ['🐻']]

animals.flat()                              // ['🐥', '🐰', '🐷', '🐻']

animals.flatMap(animal => animal + '🍌')    // ['🐥🍌', '🐰🍌', '🐷🍌', '🐻🍌']
```

# Object.fromEntries
##### for directly turning the return value of Object.entries into a new Object

```javascript
    const fruits = [['apple', '🍎'], ['banana', '🍌'], ['avocado', '🥑']]

    const someObject = Object.fromEntries(fruits)

    /* 
    someObject =  {
            apple: "🍎"
            avocado: "🥑"
            banana: "🍌"
        }
    */
```


# TrimStart & TrimEnd
##### on String.prototype as better-named alternatives to the widely implemented but non-standard String.prototype.trimLeft and trimRight built-ins.

```javascript
    const animals = '   🐻🐰🐭🐨🐔   '

    animals.trimStart() // '🐻🐰🐭🐨🐔   '
    animals.trimEnd()   // '   🐻🐰🐭🐨🐔'
```