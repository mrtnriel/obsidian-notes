1. Numbers
2. Convert Strings to Numbers
3. Arithmetic Operators
4. Arithmetic Precedence
5. Shorthand Operators
6. Increment/Decrement

___

# Numbers

Values that can be used for arithmetic operations, PHP has two types of Numbers:
- Integer - Whole Numbers
- Float - Decimal Numbers'
## Convert Strings to Numbers

This is called Type Casting. Type Casting is the process of changing a value from one data type into another

```php
// Convert String to an Integer
$strNum = "5";
$num = (int)$strNum;

// Convert String to a Float
$strPI = "3.14";
$PI = (float)$strPI;
```

Unsuccessful conversion will result into a `0` value

## Assignment Operator

Used to assign or put values to variables


| Operator | Function   | Example     |
| -------- | ---------- | ----------- |
| `=`      | Assignment | `$num = 12` |

## Arithmetic Operators

Operators that can perform mathematical equations on numbers

| Operator | Function            | Example  |
| -------- | ------------------- | -------- |
| `+`      | Addition            | 5 `+` 5  |
| `-`      | Subtraction         | 5 `-` 5  |
| `*`      | Multiplication      | 5 `*` 5  |
| `/`      | Division            | 5 `/` 5  |
| `**`     | Exponent            | 5 `**` 2 |
| `%`      | Modulus (Remainder) | 5 `%` 2  |
Operators can be applied to variables as well

```php
// Addition
$x = 5;
$y = 10;
echo $x + $y; // Answer: 15

// Subtraction
$x = 5;
$y = 10;
echo $x - $y; // Answer: -5

// Multiplication
$x = 5;
$y = 10;
echo $x * $y; // Answer: 50

// Division
$x = 10;
$y = 5;
echo $x / $y; // Answer: 2

$x = 10;
$y = 3;
echo $x / $y; // Answer: 3.3333

// Exponent
$x = 2;
$y = 3;
echo $x ** $y; // Answer: 8

//Modulo/Modulus
$x = 5;
$y = 2;
echo $x % $y; // Answer: 1
```

### Type Conversion in Arithmetic Operations

PHP automatically converts numeric strings into integers or floats when performing arithmetic operations. This is called Type Juggling.

Example 1: Automatic Type Conversion

```php
$x = "15"; // Strings
$y = 12; // Integer
echo $x + $y; // Output: 27
```

- PHP automatically converts the string `"15"` into an integer (`15`) before performing the addition.

Example 2: Explicit Type Casting

You can manually convert a value into an integer using `(int)`.

```php
$x = "Wx";
$num = (int)$x;
echo $num; // Output: 0
```

- If the string does not start with a valid numeric value, converting it to an integer results in `0`.

Example 3: Extracting Numbers from Strings

```php
$x = "25Wx";
$num = (int)$x;
echo $num; // Output: 25
```

- PHP extracts the numeric portion at the beginning of the string.
- Characters after the numeric portion are ignored during integer conversion.

Note: PHP supports automatic type conversion during arithmetic operations, but you can also use explicit type casting with `(int)` when you want to manually convert a value.

## Arithmetic Precedence

PEMDAS is followed in the order of precedence

1. Parentheses 
2. Exponent
3. Multiplication
4. Division
5. Addition
6. Subtraction

```php
$x = 5;
$y = 10;
echo ($x + $y) / $x; // Answer: 3

$x = 12;
$y = 3;
echo $x / $y + $x; // Answer: 16

$x = 2;
$y = 5;
echo $x + $y ** $x; // Answer: 9
```

## Shorthand Operators

Performs an arithmetic operator to a variable and assigns it to itself

| Operator | Usage      | Same as        |
| -------- | ---------- | -------------- |
| `+=`     | `$x += 5`  | `$x = $x + 5`  |
| `-=`     | `$x -= 5`  | `$x = $x - 5`  |
| `*=`     | `$x *= 5`  | `$x = $x * 5`  |
| `/=`     | `$x /= 5`  | `$x = $x / 5`  |
| `**=`    | `$x **= 5` | `$x = $x ** 5` |
| `%=`     | `$x %= 5`  | `$x = $x % 5`  |

```php
$x = 2;
$x += 10;
echo $x; // Answer: 12
```


## Increment / Decrement

Adds or Subtracts 1 to a variable


| Operator | Usage            | Description | How to Read                     |
| -------- | ---------------- | ----------- | ------------------------------- |
| `++`     | `++$x` or `$x++` | Adds 1      | Pre Increment or Post Increment |
| `--`     | `--$x` or `$x--` | Subtracts 1 | Pre Decrement or Post Decrement |

### Pre Increment

```php
// Prefix 
$x = 0;

echo ++$x; // Output: 1
echo $x; // Output: 1
```

Increases the value by 1 before returning or using the value.
### Post Increment

```php
// Postfix 
$x = 0;

echo $x++; // Output: 0
echo $x; // Output: 1
```

Returns or uses the current value first, then increases it by 1.