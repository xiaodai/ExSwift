#Int

### Contents ###

- [Int](#int)
    - [Instance Methods](#instance-methods)
    	- [`times`](#times)
    	- [`after`](#after)
    	- [`isEven`](#iseven)
    	- [`isOdd`](#isodd)
    	- [`upTo`](#upto)
    	- [`downTo`](#downto)
    	- [`clamp`](#clamp)
    	- [`isIn`](#isin)
    - [Class Methods](#class-methods)
    	- [`random`](#random)

### Instance Methods ###

##### `times` #####
```
3.times({ (index: Int) -> Any in println(index) })
// → 0 1 2

2.times({ println("Hello") })
// → Hello Hello
```

##### `after` #####
```
let f = 2.after({ println("Ciao") })
f()
// → 
f()
// → 
f()
// → Ciao
```

##### `isEven` #####
```
2.isEven()
// → true
```

##### `isOdd` #####
```
1.isOdd()
// → true
```

##### `upTo` #####
```
5.upTo(10, { println($0) })
// → 5 6 7 8 9 10
```

##### `downTo` #####
```
5.downTo(0, { println($0) })
// → 5 4 3 2 1 0
```

##### `clamp` #####
```
5.clamp(0...4)
// → 4

1.clamp(2...4)
// → 2
```

##### `isIn` #####
```
2.isIn(0..3)
// → true

2.isIn(0..3, strict: true)
// → false
```

### Class Methods ###

##### `random` #####
```
Int.random(min: 0, max: 10)
// → 5
```