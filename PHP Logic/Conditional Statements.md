1. if
2. if..else
3. if..elseif..else
4. switch
___

# `if` Statement

The `if` statement executes some code only if the specified condition is true.

```php
if (condition) {
  // code to be executed if condition is true;
}
```

It is common to use variables in the `if` statement:

```php
$t = 14;

if ($t < 20) {
  echo "Have a good day!"; // Output: Have a good day!
} 
```
___
# `if...else` Statement

The `if...else` statement executes some code if a condition is true and another code if that condition is false.

```php
if (condition) {
  // code to be executed if condition is true;
} else {
  // code to be executed if condition is false;
}
```

```php
$t = date("H");

if ($t < "20") {
  echo "Have a good day!";
} else {
  echo "Have a good night!"; // Output: Have a good day!
}
```

___
# `if...elseif...else` Statement

The `if...elseif...else` statement executes different codes for more than two conditions.

```php
if (condition) {
  // code to be executed if this condition is true;
} elseif (condition) {
  // code to be executed if first condition is false and this condition is true;
} else {
  // code to be executed if all conditions are false;
}
```

```php
$t = date("H");

if ($t < "10") {
  echo "Have a good morning!";
} elseif ($t < "20") {
  echo "Have a good day!";
} else {
  echo "Have a good night!"; // Output: Have a good day!
}
```
___
## Nested `if`

You can have `if` statements inside `if` statements, this is called nested `if` statements.

```php
$a = 13;

if ($a > 10) {
  echo "Above 10";
  if ($a > 20) {
    echo " and also above 20";
  } else {
    echo " but not above 20";
  }
}
```
___
# `switch` Statement

The `switch` statement is used to perform different actions based on different conditions.

Use the `switch` statement to select one of many blocks of code to be executed.

```php
switch (expression) {

  case label1:
    //code block
    break;
    
  case label2:
    //code block;
    break;
    
  case label3:
    //code block
    break;
    
  default:
    //code block
    
}
```

This is how it works:

- The expression is evaluated once
- The value of the expression is compared with the values of each case
- If there is a match, the associated block of code is executed
- The break keyword breaks out of the switch block
- The default code block is executed if there is no match

```php
$favcolor = "red";

switch ($favcolor) {

  case "red":
    echo "Your favorite color is red!";
    break;
    
  case "blue":
    echo "Your favorite color is blue!";
    break;
    
  case "green":
    echo "Your favorite color is green!";
    break;
    
  default:
    echo "Your favorite color is neither red, blue, nor green!"; // Output: Your favorite color is red!
}
```

### `break` Keyword

When PHP reaches a break keyword, it breaks out of the switch block.

This will stop the execution of code, and no more cases are tested.

The last code block does not need a break, the block breaks (ends) there anyway.

Warning: If you omit the break statement in a case that is not the last, and that case gets a match, the next case will also be executed even if the evaluation does not match the case!

### `default` Keyword

The default keyword specifies the code to run if there is no case match
___
