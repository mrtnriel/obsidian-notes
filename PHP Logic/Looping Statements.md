1. while
2. do...while
3. for
4. foreach

___
# `while` Loop

Loops through a block of code as long as the specified condition is true.

```php
while (condition) {
  // code to be executed repeatedly as long as condition is true
}
```

- **Note**: The condition is checked at the beginning of each iteration, which means that if the condition is initially false, the code block will not run even once.

```php
$i = 1; // Initialize counter
while ($i < 6) { // Check condition
  echo $i; // Execute code
  $i++; // Increment counter
}
```

- **Note:** Remember to increment the counter `($i)`, or else the loop will continue forever.

The condition does not have to be a counter, it could be the status of an operation or any condition that evaluates to either true or false.
## `break` Statement

With the `break` statement we can stop the loop even if the condition is still true

Stop the loop when `$i` is 3:

```php
$i = 1;
while ($i < 6) {
  if ($i == 3) break; 
  echo $i;
  $i++;
}
```

## `continue` Statement

With the `continue` statement we can skip the current iteration, and continue with the next

Skip, and move to the next iteration if `$i` is 3:

```php
$i = 0;
while ($i < 6) {
  $i++;
  if ($i == 3) continue;
  echo $i;
}
```

# Alternative Syntax

The `while` loop syntax can also be written with the `endwhile` statement like this

Print `$i` as long as `$i` is less than 6:

```php
$i = 1;
while ($i < 6): // Print `$i` as long as `$i` is less than 6
  echo $i;
  $i++;
endwhile;
```

___

# `do...while` Loop

Loops through a block of code at least once, and then repeats the loop as long as the specified condition is true.

```php
do {
  // code to be executed
} while (condition);
```

- **Note**: In a do...while loop the condition is tested after executing the code within the loop. This means that the loop will execute at least once, even if the condition is false.

Set `$i = 1`, then print `$i` as long as `$i` is less than 6:

```php
$i = 1; 

do {
  echo $i;
  $i++;
} while ($i < 6);
```

Here, we set the variable `$i` to 8 instead of 1, and execute the same `do...while` loop again

Set `$i = 8`, then print `$i` as long as `$i` is less than 6:

```php
$i = 8;

do {
  echo $i;
  $i++;
} while ($i < 6);
```

## `break` Statement

With the `break` statement we can stop the loop even if the condition is still true

Stop the loop when `$i` is 3:

```php
$i = 1;

do {
  if ($i == 3) break;
  echo $i;
  $i++;
} while ($i < 6);
```

## `continue` Statement

With the `continue` statement we can skip the current iteration, and continue with the next

Skip, and move to the next iteration if `$i` is 3:

```php
$i = 0;

do {
  $i++;
  if ($i == 3) continue;
  echo $i;
} while ($i < 6);
```

___

# `for` Loop

Loops through a block of code a specified number of times.

The `for` loop is used when you know how many times the script should run.

```php
for (initialization; condition; increment) {
  // code to be executed
}
```

This is how it works:

- initialization - is evaluated once (typically sets a counter variable)
- condition - is evaluated before each iteration (if true - continue loop)
- increment - is evaluated after each iteration (typically used to increase/decrease the counter variable)

The following example shows a `for` loop that prints the numbers from 0 to 10:

```php
for ($x = 0; $x <= 10; $x++) {
  echo "The number is: $x <br>";
}
```