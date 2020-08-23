# Unit 1 Lesson 2 - Statements, Expressions, Data Types and Variables

[Previous Lesson](https://github.com/Kevin-Lago/Java-Course-Guide/tree/master/unit_1_getting_started/lesson_1_introduction_to_java)

[Lesson Slides](https://docs.google.com/presentation/d/1mUUR4Sbu7yTlyrWjL2at44_BOAi9ZFxZLuGG-gCkznw/edit?usp=sharing)

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
	
- Messy code can be EXTREMELY hard to follow.
	
``` java
public class MessyCode { public static void main(String[] args) {
int[] grades = {2, 98, 58, 83, 95, 36, 36, 78, 37, 86, 85, 87, 98, 100, 38};
    int min = 100;int max = 0;
 int sum = 0;
    int mean = 0;
        double variance = 0;
    double standardDeviation = 0;
        for (int grade : grades) { if (grade > max) max = grade;
if (grade < min) min = grade;
    sum += grade; }mean = (sum / grades.length);

for (int grade : grades) {
    variance += Math.pow(num - mean, 2);
}
 variance = Math.sqrt(variance / grades.length);
standardDeviation = Math.sqrt(variance); }}
```

- Clean code is easier to change and understand

```java
public class CleanCode {
    public static void main(String[] args) {
        int[] grades = {2, 98, 58, 83, 95, 36, 36, 78, 37, 86, 85, 87, 98, 100, 38};
        int min = 100; int max = 0; int sum = 0; int mean = 0;
        double variance = 0; double standardDeviation = 0;

        for (int grade : grades) {
            if (grade > max) max = grade;
            if (grade < min) min = grade;
            sum += grade;
        }

        mean = (sum / grades.length);

	for (int num : a) {
            variance += Math.pow(num - mean, 2);
        }

        standardDeviation = Math.sqrt(variance / a.length);

        System.out.printf("%.1f %n", standardDeviation);
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
- Comments are used if code is unclear or when communicating with your team!
- Single line comments.

```java
// This is a single lined comment
```

```java
public class HelloWorld {
	// Prints Hello, World! to the console
	public static void main(String[] args) {
		System.out.println("Hello, World!");
	}
}
```

- Block comments.

```java
/*
* This is a block comment
*/
```

```java
public class HelloWorld {
    /*
    * Todo: This code needs to print a smiley face too
    * */
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
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
- bytes, shorts, ints and longs are primitive number data types.

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

- booleans are a primitive data type of either a true or false value.

```java
boolean defaultBooleanValue = false;
boolean trueBooleanValue = true;
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
- (Data Type) (Identifier)
- Lets declare a String variable with the identifier stringVariable.

```java
String stringVariable;
```

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
- Identifiers Must start with either a letter, underscore or dollar sign. 

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
- Classes and Vairables start with nouns
- Methods start with verbs

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
- [Naming Conventions - Oracle](https://www.oracle.com/java/technologies/javase/codeconventions-namingconventions.html#:~:text=Class%20names%20should%20be%20nouns,such%20as%20URL%20or%20HTML)
- [Java Naming Conventions - javatpoint](https://www.javatpoint.com/java-naming-conventions)

---
## Expressions

- “An expression is a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value.” - Oracle Java Docs
- Basically some code that equates to a single value.

### Helpful Links

to read

- [Oracle Docs Expressions, Statements and Blocks](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/expressions.html)
- [Java Expressions Introduced - Paul Leahy](https://www.thoughtco.com/expression-2034097#:~:text=Expressions%20are%20essential%20building%20blocks,variables%2C%20operators%20and%20method%20calls.)

---
## Statements

- A Statement is like a full sentence.
- We can turn an Expression into an Expression Statement using a ;

```java
int intVariable = 5;
```

- We can also use Control Flow Statements which will be covered in unit 1 lesson 3
- Control Flow Statement examples:
	- if
	- else if
	- else
	- for
	- while

### Helpful Links

to read

- [Oracle Docs Expressions, Statements and Blocks](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/expressions.html)

---
## Operators

- Arithmetic Operators: +, -, *, /, %, ++, --
- Arithemtic Operators allow us to do basic math

| Operator |  Name                    | Function                                     | Example       | Result Value |
|:--------:|:------------------------:|----------------------------------------------|---------------|--------------|
| +        | Addition Operator        | Adds two values                              | int x = 2 + 2 | 4            |
| -        | Subtraction Operator     | Subtracts two values                         | x = x - 2     | 2            |
| *        | Multiplication Operator  | Multiplies two values                        | x = x * 3     | 6            |
| /        | Division Operator        | Divides two values                           | x = x / 2     | 3            |
| %        | Modulus Operator         | Divides two values and returns the remainder | x = x % 2     | 1            |
| ++       | Increment Operator       | Adds 1 to a value                            | x++           | 2            |
| --       | Decrement Operator       | Subtracts 1 from a value                     | x--           | 1            |

- Assignment Operator: =, +=, -=, *=, /=, %=
- Assignment Operators asign a value to a Variable
	
| Operator |  Name                    | Function                                          | Example       | Result Value |
|:--------:|:------------------------:|---------------------------------------------------|:-------------:|--------------|
| =        | Equals Operator          | Assigns a value to a Variable                     | int x = 2     | 2            |
| +=       | Plus-Equals Operator     | Adds a value to a Variables original value        | x += 6        | 8            |
| -=       | Minus-Equals Operator    | Subtracts a value from a Variables original value | x -= 2        | 6            |
| *=       | Multiply-Equals Operator | Multiplies a value to a Variables original value  | x *= 2        | 12           |
| /=       | Divide-Equals Operator   | Divides a value from a Variables original value   | x /= 4        | 3            |
| %=       | Modulus-Equals Operator  | Returns the remainder of a Variables value        | x %= 2        | 1            |

- Relational/Comparison Operators: <, <=, >, =>, ==, !=
- Relational/Comparison Operators allow us to compare two values
- Relational/Comparison Operators will equate a true or false value

| Operator |  Name                           | Function                                          | Example | Result Value |
|:--------:|:-------------------------------:|---------------------------------------------------|:-------:|--------------|
| <        | Less-Than Operator              | Returns true if a is less than b                  | 2 < 4   | true         |
| <=       | Less-Than-Or-Equals Operator    | Returns true if a is less than or equal to b      | 2 <= 3  | false        |
| >        | Greater-Than Operator           | Returns true if a is greater than b               | 3 > 2   | true         |
| >=       | Greater-Than-Or-Equals Operator | Returns true if a is greater than or equal to b   | 3 >= 3  | true         |
| ==       | Does-Equal Operator             | Returns true if a does equal b                    | 3 == 3  | true         |
| !=       | Does-Not-Equal Operator         | Returns true if a does not equal b                | 2 != 2  | false        |

- Logical Operators: &&, ||, !

- Bitwise Operators: &, |, ~, ^, <<, >>, >>>

### Helpful Links

to read

- [w3schools Java Operators](https://www.w3schools.com/java/java_operators.asp)
- [Oracle Docs Assignment, Arithmetic and Unary Operators](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op1.html#:~:text=One%20of%20the%20most%20common,the%20operand%20on%20its%20left%3A&text=This%20operator%20can%20also%20be,as%20discussed%20in%20Creating%20Objects.)

---
## Activities

- Familiarize yourself with Java Keywords!
- Familiarize yourself with Javas Primtive Data Types!
- Do some Math!

### Helpful Links

to read

- []()

to watch

- []()

---

[Lesson Quiz]()

[Next Lesson](https://github.com/Kevin-Lago/Java-Course-Guide/tree/master/unit_1_getting_started/lesson_3_loops_and_logic)

# Full Java Course

<a href="https://github.com/Kevin-Lago/java_full_course">
	<img src="../../java_logo.png" />
</a>


