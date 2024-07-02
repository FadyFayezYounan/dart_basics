# Dart Control Flow Statements

Control flow statements are fundamental in any programming language as they dictate the flow of program execution.Dart provides several control flow statements to help you manage the flow of your code efficiently.

## 1. Conditional Statements

### a. `if` and `else`

The `if` statement is used to execute a block of code if a specified condition is true. The `else` statement can be used to execute a block of code if the condition is false.

```dart
  int age = 20;

  if (age >= 18) {
    print('You are an adult.');
  } else {
    print('You are a minor.');
  }
```

### b. `if-else-if`

The `else if` statement allows you to check multiple conditions before executing a block of code.

```dart
  int score = 85;

  if (score >= 90) {
    print('Grade: A');
  } else if (score >= 80) {
    print('Grade: B');
  } else if (score >= 70) {
    print('Grade: C');
  } else {
    print('Grade: F');
  }
```

### c. Ternary Operator

The ternary operator is a shorthand way of writing an `if-else` statement.

```dart
  int age = 20;
  String eligibility = age >= 18 ? 'Eligible to vote' : 'Not eligible to vote';
  print(eligibility); // Output: Eligible to vote
```

## 2. Switch Statement

The `switch` statement evaluates an expression, matches the expression's value to a case clause, and executes the associated block of code.

```dart
 String grade = 'B';

  switch (grade) {
    case 'A':
      print('Excellent!');
      break;
    case 'B':
      print('Good job!');
      break;
    case 'C':
      print('Well done');
      break;
    case 'D':
      print('You passed');
      break;
    case 'F':
      print('Better try again');
      break;
    default:
      print('Invalid grade');
  }
```

## 3. Loops

### a. `for` Loop

The `for` loop is used to iterate over a sequence (such as a list or a range) and execute a block of code multiple times.

```dart
  List<int> numbers = [1, 2, 3, 4, 5];

  for (int i = 0; i < numbers.length; i++) {
    print(numbers[i]); // Output: 1, 2, 3, 4, 5
  }
```

### b. `for-in` Loop

The `for-in` loop is a simplified version of the for loop, specifically used to iterate over elements in a collection.

```dart
  List<String> fruits = ['Apple', 'Banana', 'Cherry'];

  for (String fruit in fruits) {
    print(fruit); // Output: Apple, Banana, Cherry
  }
```

### c. `while` Loop

The `while` loop executes a block of code as long as a specified condition is true.

```dart
  int count = 0;

  while (count < 5) { // Loop will execute 5 times
    print(count); // Output: 0, 1, 2, 3, 4
    count++;
  }
```

### d. `do-while` Loop

The `do-while` loop is similar to the `while` loop, but it executes a block of code at least once, and then repeats the loop as long as a specified condition is true.

```dart
  int count = 0;

  do {
    print(count); // Output: 0, 1, 2, 3, 4
    count++;
  } while (count < 5);
```

### e. `break` and `continue`

The `break` statement is used to exit a loop prematurely, while the continue statement skips the rest of the code inside the loop for the current iteration and jumps to the next iteration.

```dart
  for (int i = 0; i < 10; i++) {
    if (i == 8) {
      break; // Exit the loop when i is 5
    }
    if (i % 2 == 0) {
      continue; // Skip even numbers
    }
    print(i); // Output: 1, 3, 5, 7
  }
```

## 4. Exception Handling

Dart provides a robust exception handling mechanism using `try`, `catch`, `on`, and `finally` blocks.

### a. `try` and `catch` Blocks

Use `try` to wrap code that might throw an exception, and `catch` to handle the exception.

example: Make a function that used to divide two numbers and catch the exception if it occurs.

```dart
  int divide(int a, int b) {
    try {
      // `~/` is the integer division operator
      // because `a` divided by `b` returns a `double` value
      // but we need an `int` value here
      // so we use `~/` to convert the `double` value to `int` value
      return a ~/ b;
    } catch (e) {
      print('Error: $e');
      return 0;
    }
  }

  int result = divide(10, 0); // Output: Error: IntegerDivisionByZeroException
  print(result); // Output: 0
```

### b. `on` and `catch`

The `on` keyword can be used to specify the type of exception to catch.

```dart
  int divide(int a, int b) {
    try {
      // `~/` is the integer division operator
      // because `a` divided by `b` returns a `double` value
      // but we need an `int` value here
      // so we use `~/` to convert the `double` value to `int` value
      return a ~/ b;
    } on IntegerDivisionByZeroException { // UnsupportedError
      print('Error: Cannot divide by zero.');
      return 0;
    } catch (e) {
      print('Error: $e');
      return 0;
    }
  }

  int result = divide(10, 0); // Output: Error: IntegerDivisionByZeroException
  print(result); // Output: 0
```

### c. `finally`

The `finally` block is executed regardless of whether an exception is thrown or not.

```dart
  int divide(int a, int b) {
    try {
      // `~/` is the integer division operator
      // because `a` divided by `b` returns a `double` value
      // but we need an `int` value here
      // so we use `~/` to convert the `double` value to `int` value
      return a ~/ b;
    } on IntegerDivisionByZeroException { // UnsupportedError
      print('Error: Cannot divide by zero.');
      return 0;
    } catch (e) {
      print('Error: $e');
      return 0;
    } finally {
      print('This code always runs.');
    }
  }
```
