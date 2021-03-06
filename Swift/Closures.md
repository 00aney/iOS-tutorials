#Closures

```swift
func makeIncrementer(forIncrement amount: Int) -> () -> Int {
  var runningTotal = 0
  func incrementer() -> Int {
    runningTotal += amount
    return runningTotal
  }
  return incrementer
}
```

The nested ```incrementer()``` function captures two values, ```runningTotal``` and ```amount```.

```makeIncrementer``` returns ```incrementer```

```incrementer``` is a closure that increments ```runningTotal``` by amount each time it is called.


###example
```swift
let incrementByTen = makeIncrementer(forIncrement: 10)

incrementByTen()  // returns a value of 10
incrementByTen()  // returns a value of 20
incrementByTen()  // returns a value of 30
```
