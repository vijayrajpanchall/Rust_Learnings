# Rust Learning

This repository contains information and resources for learning Rust programming language.

## Why Rust

- High-level language features without performance penalties.
- Program behaviors can be enforced at compile time, enhancing program reliability.
- Built-in dependency management, similar to npm.
- Quickly growing ecosystem of libraries.
- Friendly and welcoming developer community.

## Technical Rust Goodies

### First-Class Multithreading

- **Multithreading:** Multithreading in programming is like being a master chef who can multitask effortlessly, preparing multiple dishes simultaneously. It allows programs to divide their workload into independent threads, improving performance by executing tasks concurrently. However, proper synchronization is necessary to avoid conflicts and ensure smooth cooperation among threads.
- Compiler error to improperly access shared data.

### Type System

- Can uncover bugs at compile time.
- Makes refactoring simple.
- Reduces the number of tests needed.

### Module System

- Makes code separation simple.

### Adding a Dependency

- Adding a dependency is only one line in a config file.

### Tooling

- Generate docs, lint code, auto format.

### Rust is Different by Design

- "Clean slate" approach.
- Important because of subtle language differences between Rust and others.
- Helps facilitate learning Rust.
- Plenty of coding exercises for becoming familiar with Rust code.

## Data Types

- Memory only stores binary data.
- Anything can be represented in binary.
- Program determines what the binary represents.
- Basic types that are universally useful are provided by the language.



## Variables


## Functions

- A way to encapsulate program functionality.
- Optionally accept data.
- Optionally return data.
- Utilized for code organization.
- Also makes code easier to read.


`i32` represents a 32-bit integer.

### `println!` Macro

- Macros use an exclamation point to call/invoke.
- Generate additional Rust code.
- Data can be printed using `println!`:
    - `{:?}`
    - `{variableName}`

### Match

- Adds logic to the program.
- Similar to `if...else`.
- Exhaustive - all options must be accounted for.

#### Match vs IF...ELSE

- Match will be checked by the compiler.
- If a new possibility is added, you will be notified when this occurs.
- `else if` is not checked by the compiler.
- If a new possibility is added, your code may contain a bug.

### Enum - Enumeration

- Data that can be one of multiple different possibilities.
- Each possibility is called a "variant".
- Provides information about your program to the compiler.
- Makes the program more robust when paired with match.
- Makes the program easier to read.

**Advanced**

- Enum variants can optionally contain data.
- The data can be another enum.
- Can mix plain identifiers and data-containing variants within the same enum.
- More than one piece of data can be associated with a variant.


### Struct

- A type that contains multiple pieces of data.
- All fields must be present to create a struct.
- Each piece of data is called a "field".
- Makes working with data easier.
- Similar data can be grouped together.


### Tuples

- A type of "record".
- Store data anonymously.
- No need to name fields.
- Useful to return pairs of data from functions.
- Can be "destructured" easily into variables.


### Expressions

- Rust is an expression-based language.
- Most things are evaluated and return some value.
- Expression values coalesce to a single point.
- Can be used for nesting logic.

### Memory

- Memory is stored using binary.
- Bits: 0 or 1.
- Computer optimized for bytes.
- 1 byte = 8 contiguous bits.
- Fully contiguous.

### Addresses

- All data in memory has an "address".
- Used to locate data.
- Address remains the same, only data changes.
- Usually, addresses are not utilized directly.
- Variables handle most of the work.

### Offsets

- Items can be located at an address using offsets.
- Offsets begin at 0.
- Represents the number of bytes away from the original address.
- Normally deal with indexes instead.

### Ownership - Managing Memory

- Programs must track memory.
- If they fail to do so, a "leak" occurs.
- Rust utilizes an "ownership" model to manage memory.
- The owner of memory is responsible for cleaning up the memory.
- This occurs automatically at the end of the scope.
- Memory can either be "moved" or borrowed.
- Default behavior is to move memory to a new owner.
- Use an `&` to allow code to borrow memory.

#### Borrow Example


### Vector

Vectors are a data structure in Rust that represent a sequence of values. They are similar to arrays, which are also used to store multiple values in a single data structure. However, unlike arrays, vectors have the ability to grow or shrink dynamically as needed.

- Contain multiple pieces of data (must be the same type).
- Used for lists of information.
- Can add, remove, and traverse the entries.
- The `vec!` macro can be used to make vectors.
- Use `for..in` to iterate through items of a vector.

### String and &str

- Two commonly used types of strings.
    - `String` - owned.
    - `&str` - borrowed string slice.
- Must use an owned string to store in a struct.
- Use `&str` when passing to a function.


## Conclusion

Rust is a powerful and modern programming language that provides memory safety, concurrency, and performance. It offers a unique combination of high-level language features and low-level control. By leveraging its type system, ownership model, and extensive tooling, developers can build robust and efficient software systems.

If you're interested in learning Rust, this repository provides a comprehensive collection of resources, examples, and exercises to help you get started. Feel free to explore the code, experiment, and dive deeper into the world of Rust programming.

Happy coding!
