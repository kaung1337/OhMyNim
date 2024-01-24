### Nim Basics:

1. **Hello World:**

```jsx
echo "Hello, World!"
```

- **Variables:**

```jsx
var myVar: int = 42 let myConstant: string = "immutable"
```

- **Control Flow:**

```jsx
if condition: # code elif anotherCondition: # code else: # code for i in 0..<10: # code while condition: # code
```

- **Procedures (Functions):**

```jsx
proc add(x, y: int): int = result = x + y
```

- **Strings:**

```jsx
let myString = "Nim Programming" echo myString[0] # accessing individual characters
```

### Advanced Features:

1. **Sequences (Arrays):**

```jsx
var myArray: array[3, int] = [1, 2, 3] echo myArray[1] # accessing array element
```

- **Tuples:**

```jsx
let myTuple = (1, "hello", 'c') echo myTuple[0]
```

- **Enums:**

```jsx
type MyEnum = enum A, B, C var myVar: MyEnum = MyEnum.B
```

- **Case Statements:**

```jsx
case myVar of MyEnum.A: # code of MyEnum.B: # code else: # code
```

1. **Exception Handling:**

```
try:
  # code
except MyException:
  # handle exception
finally:
  # code to execute regardless of exceptions

```

### Modules and Packages:

1. **Importing Modules:**

```jsx
import math let sqrt2 = sqrt(2.0)
```

- **Creating Modules:**

```
# mymodule.nim
module mymodule
proc myFunction() =
  # code

```

```jsx
# main.nim import mymodule myFunction()
```

- **Command-Line Arguments:**

```jsx
import commandLine let arg1 = commandLine[1]
```

- **File I/O:**

```jsx
var file = open("myfile.txt", fmWrite) write(file, "Hello, File!") close(file)
```

- **Concurrency (Async/Await):**

```
import asynchttpclient

proc fetchData(url: string): Future[string] {.async.} =
  # async code to fetch data

proc main() {.async.} =
  let data = await fetchData("<https://evil.com>")
  echo data

waitFor main()

```
