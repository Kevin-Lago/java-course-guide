# Unit 1 Lesson 3 - Loops and Logic

[Previous Lesson](https://github.com/Kevin-Lago/full_java_course/tree/master/unit_1/lesson_2_statements_expressions_datatypes_and_variables)

[Lesson Slides]()

---
## Program Flow

- Like a list of instructions code is read from left to right, top to bottom.

	- Go forward 2 steps
	- Turn left 90 degrees
	- Go backwards 5 steps
	- Turn right 180 degrees

- We can control flow using methods, loops and logic.

	- Go forward 2 steps
	- Repeat the first instruction 3 times
	- Turn left 90 degrees
	- Go backwards 5 steps
	- If we're facing north go back to step one
	- Turn right 180 degrees

### Helpful Links

to read

- []()

to watch

- []()

---
## Boolean Expressions

- Helps us make decisions
- Allows us to control the flow of a program
- Used for testing conditions
	- Relational
	- Conditional
	
```java
boolean theSunIsHot = true;
boolean iceMelts = true;
boolean applesAreAVegetable = false;
boolean blueIsRed = false;
```

### Helpful Links

to read

- []()

to watch

- []()

---
## Relational Operators

- == (equals)
- <, > (greater than, less than)
- != (not equals)
- <=, >= (greater than or equal, less than or equal)

- We use relational operators to compare values in conjunction with conditional statements and loops.

```java
boolean equalsExample1 = 50 == (5 * 10); // true
boolean equalsExample2 = 49 == (5 * 10); // false
boolean lessThanExample1 = 2 < 4; // true
boolean lessThanExample2 = 6 < 4; // false
boolean greaterThanExample1 = 7 > 5; // true
boolean greaterThanExample2 = 1 > 5; // false
boolean doesNotEqualExample1 = 6 != 1; // true
boolean doesNotEqualExample2 = 1 != 1; // false
boolean lessThanOrEqualToExample1 = (10 * 5) <= (60 - 10); // true
boolean lessThanOrEqualToExample2 = (10 * 10) <= (60 - 10); // false
boolean greaterThanOrEqualToExample1 = (10 * 5) >= (60 - 10); // true
boolean greaterThanOrEqualToExample2 = (2 * 3) >= (60 - 10); // false
```

### Helpful Links

to read

- [Equality, Relational and Conditional Operators - Oracle Docs](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op2.html)
- [Java Realational Operators with Examples - GeeksforGeeks](https://www.geeksforgeeks.org/java-relational-operators-with-examples/)
- [Java Operators - w3schools](https://www.w3schools.com/java/java_operators.asp)

to watch

- []()

---
## if Statements

- An if statement will run a block of code if a condition is met.
- The condition will be checked inside the if's parentheses. ()
- The block of code that will be run resides within the curly brackets. {}

```java
if (condition) {
	// execute this code if condition is true
}
```

```java
if (5 > 2) {
	System.out.print("This will be printed to the console");
}
```

```java
if (5 < 2) {
	System.out.print("This will not be printed to the console");
}
```

### Helpful Links

to read

- []()

to watch

- []()

---
## if, else Statements

- The else statement will run a block of code for every condition that isnt true.

```java
if (condition) {
	// execute this code if condition is true
} else {
	// execute this code if condition is false
}
```

```java
if ((5 * 4) > 10) {
	System.out.print("This will be printed to the console");
} else {
	System.out.print("This will not be printed to the console");
}
```

```java
if (5 < (2 / 2)) {
	System.out.print("This will not be printed to the console");
} else {
	System.out.print("This will be printed to the console");
}
```

### Helpful Links

to read

- []()

to watch

- []()

---
## if, else if, else Statements

- The else if statement allows us to check for other conditions

```java
if (condition) {
	// execute this code if condition is true
} else if (anotherCondition) {
	// execute this code if anotherCondition is true
} else {
	// execute this code if no conditions are true
}
```

```java
if ((5 * 8) >= (5 * 8)) {
	System.out.print("This will be printed to the console");
} else if (anotherCondition) {
	System.out.print("This will not be printed to the console");
} else {
	System.out.print("This will not be printed to the console");
}
```

```java
if (8 <= 2) {
	System.out.print("This will not be printed to the console");
} else if (8 >= 2) {
	System.out.print("This will be printed to the console");
} else {
	System.out.print("This will not be printed to the console");
}
```

```java
if (8 <= 2) {
	System.out.print("This will not be printed to the console");
} else if (8 >= 48) {
	System.out.print("This will not be printed to the console");
} else {
	System.out.print("This will be printed to the console");
}
```

- We can have multiple else if statements.

```java
if (8 <= 2) {
	System.out.print("This will not be printed to the console");
} else if (8 >= 48) {
	System.out.print("This will not be printed to the console");
} else if (8 <= 2) {
	System.out.print("This will not be printed to the console");
} else if (8 == 8) {
	System.out.print("This will be printed to the console");
} else {
	System.out.print("This will not be printed to the console");
}
```

### Helpful Links

to read

- []()

to watch

- []()

---
## switch Statements

### Helpful Links

to read

- []()

to watch

- []()


---
## Loops

- Loops allow us to repeat a block of code.
- We can use for loops

```java
// This writes "Hello, World!" 5 times to the terminal
for (int i = 0; i < 5; i++) {
	System.out.println("Hello, World!");
}
```

- And we can use while loops

```java
// This writes "Hello, World!"
while () {
	System.out.println("Hello, World!");
}
```

- There're also enhanced for loops which will be covered in lesson 6 - Arrays

### Helpful Links

to read

- []()

to watch

- []()

---
## Activities

- Calculator and Random Numbers
- 

### Helpful Links

to read

- []()

to watch

- []()

---

[Lesson Quiz]()

[Next Lesson](https://github.com/Kevin-Lago/full_java_course/tree/master/unit_1/lesson_4_objects_and_methods)

# Full Java Course

<a href="https://github.com/Kevin-Lago/java_full_course">
	<img src="../../java_logo.png" />
</a>


