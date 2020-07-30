# Unit 1 Lesson 2 - Statements, Expressions, Data Types and Variables

[Previous Lesson](https://github.com/Kevin-Lago/Java-Course-Guide/tree/master/unit_1_getting_started/lesson_1_introduction_to_javahttps://github.com/Kevin-Lago/Java-Course-Guide/tree/master/unit_1_getting_started/lesson_1_introduction_to_java)

---
## Write Clean Code!

- Writing clean code is vital for working with others and your future self.
- Writing code cleanly and with style are two different things.

``` java
// Clean code
public class HelloWorld {
	public static void main(String[] args) {
		System.out.println("Hello, World!");
	}
}
```

``` java
// Clean code different style
public class HelloWorld 
{
	public static void main(String[] args) 
	{
		System.out.println("Hello, World!");
	}
}
```
	
- Writing messy code can ARGUABLY be faster but will waste alot of time.
	
``` java
 public class  HelloWorld 
	{public static void main(String[]  args) 
  {System.out.println("Hello, World");
	   }
	}
```

### Helpful Links

to read

- [Amazon: Clean Code - Robert C. Martin](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882#:~:text=From%20the%20Publisher&text=Best%20agile%20practices%20of%20cleaning,practices%20of%20true%20software%20craftsmanship.)
- [Clean, High Quality Code - Arash Arabi](https://www.butterfly.com.au/blog/website-development/clean-high-quality-code-a-guide-on-how-to-become-a-better-programmer)

to watch

- [10 Tips For Clean Code - Michael Toppa](https://www.youtube.com/watch?v=UjhX2sVf0eg)
- [Effective and Clean Java Code - Edson Yanaga](https://www.youtube.com/watch?v=uOrk8mZmjaM)

---
## Comments

- Comments are ignored bits of code.
- Comments are for your team, and your future self!
- Single line comments.

```java
// This is a single lined comment
```

- Block comments.

```java
/*
This is a block comment
*/
```

### Helpful Links

to read

- [Java Comments - w3schools](https://www.w3schools.com/java/java_comments.asp)
- [Java Comments - geeksforgeeks](https://www.geeksforgeeks.org/comments-in-java/)

---
## Java Keywords

- Java Keywords are reserved words.
- These keywords are predefined and cannot be used as identifiers.
- All primitive data types are Java Keywords.
- Other keywords include for, while, if, final, static, try, ect..

### Helpful Links

to read

- [Java Keywords - Oracle Docs](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/_keywords.html)
- [Java Keywords - javatpoint](https://www.javatpoint.com/java-keywords)
- [Java Keywords - wiki](https://en.wikipedia.org/wiki/List_of_Java_keywords)

---
## Data Types

- In Java there're primitive data types and objects.
- bytes, shorts, ints, longs, floats, and doubles are primitive number data types.

```java
byte byteMinimumValue = -128;
byte defaultByteValue = 0;
byte byteMaximumValue = 127;
```
```java
short shortMinimumValue = -32768;
short defaultShortValue = 0;
short shortMaximumValue = 32767;
```
```java
int intMinimumValue = -2147483648;
int intDefaultValue = 0;
int intMaximumValue = 2147483647;
```
```java
long longMinimumValue = -9223372036854775808;
long defaultLongValue = 0;
long longMaximumValue = 9223372036854775807;
```

- floats and doubles are primitive number values with a decimal place.

```java
float floatValue1 = 5.7f;
float floatValue2 = 247.963f;
float defaultFloatValue = 0.0f;
```
```java
double doubleValue1 = 8.8d;
double doubleValue2 = 5937.3276d;
double defaultDoubleValue = 0.0d;
```

- booleans are a primitive data type with either a true or false value.

```java
boolean defaultBooleanValue = false;
```

- chars are a single letter.
- Unlike Strings we use single quotation marks for chars.

```java
char a = 'a';
char b = 'b';
char c = 'c';
char defaultCharValue = '\u0000';
```

- Objects are not primitives and make up the rest of the data types.
- Notice how object data types are capitalized while primtive data types are not.

```java
String defaultStringValue = null;
String string = "This is an Object";
Object defaultObjectValue = null;
```

### Helpful Links

to read

- [Java Data Types - w3schools](https://www.w3schools.com/java/java_data_types.asp)
- [Oracle Docs Primitive Data Types](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)

---
## Variables

- Variables are named bits of computer memory in which you can store a value.
- Variables first need a data type and then a name:
- <Data Type> <Identifier>

```java
String stringVariable;
```

- Here we're declaring a String variable with the identifier stringVariable.
- Declaring a variable only reserves the memory; it doesn’t put anything in the memory. For that, we need to assign a value to our new variable.
- We assign values to our variables using the assignment operator (=)

```java
String stringVariable = "Any String Value";
```

### Helpful Links

to read

- [w3schools Java Variables](https://www.w3schools.com/java/java_variables.asp)
- [javatpoint Java Variable](https://www.javatpoint.com/java-variables)

---
## Identifiers and Naming Conventions

- Identifiers are developer defined names for Variables, Methods and Classes.
- Identifiers cannot span multiple lines or contain spaces.
- Identifiers can only contain numbers, letters, underscores, dashes and dollar signs.
- Identifiers cannot start with a number.

```java
int exampleInt_1 = 0;
int exampleInt_2 = 0;
int exampleInt_3 = 0;

long _long$23 = 675;
```

- The first word in an identifier for Variables and Methods should be lowercase.
- The first word in an identifier for Classes should be uppercase.

```java
public class ExampleClassIdentifier {

	private String exampleVariableIdentifier;
	
	private void exampleMethodIdentifier() {}

}
```

- Names should be descriptive
- Classes and Vairables are nouns
- Methods are verbs

```java
public class Apple {

	private String color = "red";
	private int ageInSeconds = 0;
	
	private void increaseAge() {
		this.ageInSeconds++;
	}

}
```

### Helpful Links

to read

- [Geeks for Geeks Identifiers](https://www.geeksforgeeks.org/java-identifiers/)
- []()

---
## Expressions

- An Expression is like a full sentence.
- Basically some code that equates to a single value.

### Helpful Links

to read

- [Oracle Docs Expressions, Statements and Blocks](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/expressions.html)
- [Java Expressions Introduced - Paul Leahy](https://www.thoughtco.com/expression-2034097#:~:text=Expressions%20are%20essential%20building%20blocks,variables%2C%20operators%20and%20method%20calls.)

---
## Operators

- Arithmetic Operators: +, -, *, /, %

- Assignment Operator: =, +=, -=, *=, /=, %=, &=, |=, ^=, >>=, <<=

- Relational Operators: <, <=, >, =>, ==, !=

- Logical Operators: &&, ||, !

- Bitwise Operators: &, |, ~, ^, <<, >>, >>>

### Helpful Links

to read

- [w3schools Java Operators](https://www.w3schools.com/java/java_operators.asp)
- [Oracle Docs Assignment, Arithmetic and Unary Operators](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op1.html#:~:text=One%20of%20the%20most%20common,the%20operand%20on%20its%20left%3A&text=This%20operator%20can%20also%20be,as%20discussed%20in%20Creating%20Objects.)

---
## Activities

- Familiarize yourself with Java Keywords!
- Familiarize yourself with Javas primtive data types
- Create Java Calculator

### Helpful Links

to read

- []()

to watch

- []()

---

[Next Lesson](https://github.com/Kevin-Lago/full_java_course/tree/master/unit_1_getting_started/lesson_3_loops_and_logic)

# Full Java Course

<a href="https://github.com/Kevin-Lago/java_full_course">
	<img src="../../java_logo.png" />
</a>


