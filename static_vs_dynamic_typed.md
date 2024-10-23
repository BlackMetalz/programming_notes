The difference between statically typed and dynamically typed languages lies in when type checking is performed and how strict the type system is.

### Statically Typed Languages
- **Type Checking**: Performed at compile time.
- **Examples**: C++, Java, Go.
- **Advantages**:
  - **Early Error Detection**: Errors related to types are caught during compilation, reducing runtime errors.
  - **Performance**: Generally faster execution because type information is known at compile time, allowing for optimizations.
  - **Tooling**: Better support for IDE features like autocompletion and refactoring.
  - **Data Integiry**
- **Disadvantages**:
  - **Verbosity**: Often requires more code to declare types explicitly.
  - **Flexibility**: Less flexible in terms of changing types dynamically.

- **Code Example**:
```Go
package main

import "fmt"

// add function that takes two integers as arguments
func add(a int, b int) int {
    return a + b
}

func main() {
    // Correct usage
    // result := add(1, 2)
    // fmt.Println("Result:", result)

    //Incorrect usage - Uncommenting the following line will cause a compile-time error
    result = add(1, "two")
}
```

### Dynamically Typed Languages
- **Type Checking**: Performed at runtime.
- **Examples**: Python, JavaScript, Ruby.
- **Advantages**:
  - **Flexibility**: More flexible and easier to write quick scripts or prototypes.
  - **Conciseness**: Less boilerplate code since types do not need to be declared explicitly.
  - **Easy to write**: Less time to learn than static typed
- **Disadvantages**:
  - **Runtime Errors**: Type-related errors are only caught during execution, which can lead to runtime failures.
  - **Performance**: Generally slower execution due to type checking at runtime.
  - **Tooling**: Less robust IDE support for features like autocompletion and refactoring.
- **Code Example**:
```js
function add (a,b) {
  return a+b;
}

add (3,4) => 7
add (1, "three") => 1three
```

### Which is Better?
- **Use Case Dependent**: The choice between static and dynamic typing depends on the specific use case and requirements.
  - **Statically Typed**: Better for large, complex systems where early error detection and performance are critical.
  - **Dynamically Typed**: Better for rapid development, scripting, and situations where flexibility is more important than performance.

### Summary
- **Statically Typed**: Early error detection, better performance, more verbose.
- **Dynamically Typed**: More flexible, concise, potential for runtime errors.

Both have their own strengths and weaknesses, and the best choice depends on the specific needs of the project.
