### Nim Basics:

1. **Hello World:**
    
    ```
    nim
    
    ```
    
- `echo "Hello, World!"`
- **Variables:**
    
    ```
    nim
    
    ```
    
- `var myVar: int = 42
let myConstant: string = "immutable"`
- **Control Flow:**
    
    ```
    nim
    
    ```
    
- `if condition: # code
elif anotherCondition: # code
else: # code
for i in 0..<10: # code
while condition: # code`
- **Procedures (Functions):**
    
    ```
    nim
    
    ```
    
- `proc add(x, y: int): int = result = x + y`
- **Strings:**
    
    ```
    nim
    
    ```
    
1. `let myString = "Nim Programming"
echo myString[0] # accessing individual characters`

### Advanced Features:

1. **Sequences (Arrays):**
    
    ```
    nim
    
    ```
    
- `var myArray: array[3, int] = [1, 2, 3]
echo myArray[1] # accessing array element`
- **Tuples:**
    
    ```
    nim
    
    ```
    
- `let myTuple = (1, "hello", 'c')
echo myTuple[0]`
- **Enums:**
    
    ```
    nim
    
    ```
    
- `type MyEnum = enum A, B, C
var myVar: MyEnum = MyEnum.B`
- **Case Statements:**
    
    ```
    nim
    
    ```
    
1. `case myVar
of MyEnum.A: # code
of MyEnum.B: # code
else: # code`
2. **Exception Handling:**

```
nim

```

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
    
    ```
    nim
    
    ```
    
- `import math
let sqrt2 = sqrt(2.0)`
- **Creating Modules:**
    
    ```
    nim
    
    ```
    

```
# mymodule.nim
module mymodule
proc myFunction() =
  # code

```

```
nim

```

- `# main.nim
import mymodule
myFunction()`
- **Command-Line Arguments:**
    
    ```
    nim
    
    ```
    
- `import commandLine
let arg1 = commandLine[1]`
- **File I/O:**
    
    ```
    nim
    
    ```
    
- `var file = open("myfile.txt", fmWrite)
write(file, "Hello, File!")
close(file)`
- **Concurrency (Async/Await):**
    
    ```
    nim
    
    ```
    

```
import asynchttpclient

proc fetchData(url: string): Future[string] {.async.} =
  # async code to fetch data

proc main() {.async.} =
  let data = await fetchData("https://evil.com")
  echo data

waitFor main()
```
