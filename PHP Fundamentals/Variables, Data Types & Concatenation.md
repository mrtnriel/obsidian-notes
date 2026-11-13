
1. Variables
2. Data Types
3. Concatenation
___
# Variables

Variables are named storage containers used to hold data, such as text, numbers, arrays, and objects.

It is called an **Identifier**

## Identifiers

An Identifier is a variable name that has been set by the programmer

Rules to follow when declaring a variable:

1. Identifiers MUST start with a `$`
2. Identifiers MUST NOT start with a number after the `$`
3. Identifiers MUST be UNIQUE
4. Identifiers are CASE SENSITIVE
5. RESERVE KEYWORDS are NOT allowed as Identifiers
6. Identifiers CANNOT contain SPECIAL CHARACTERS except for `_` (underscore)

### Valid Identifiers

```php 
$x = "Value";
$number = 5;
$name = "David"
$name_1 = "Alenere"
```

### Invalid Identifiers

```php
x = "Value";
$echo = 5;
$n@me = "David"
$1_name = "Alenere"
```

## Declaring Variables

Uses `$` at the beginning then its Intended Identifier, an Initial Value is assigned using the `=` Operator

```php
<?php
	$x = 5;
	$y = 12.5;
	$z = "Hello World";
?>
```
___
# Data Types

The type of data that the variable is currently holding

1. String
2. Integer
3. Float
4. Boolean 
5. Array 
6. Object
7. NULL
8. Resource

```php
// String - Text
$name = "Gabriel Martin";

// Integer - Whole numbers
$number = 5;

// Float - Decimals
$decimal = 3.14;

// Boolean - True or False
$isCoding = false;
```

## Echo Variables

Display variables by using `echo`

```php
$name = 'Gabriel';
echo $name;
echo "<br>";

$age = 20;
echo $age;
echo "<br>";

$isTall = true;
echo $isTall;
```

- Note: `echo` displays `1` for `true` and an empty string for `false`.

## Var_Dump Variables

Display variable's data type by using `var_dump`

```php
var_dump($name);

var_dump($age);

var_dump($isTall);
```

An easier way to do this is by separating them with a comma

```php
var_dump($name, $age, $isTall);
```

___ 

# Concatenation

Joining two or more strings together

```php
"Hello" . "World"
"Answer :" . 12
"PI :" . 3.14
```

You can use variables and concatenate them

```php
$name = "Martin";
echo "Hi, " . $name
```

```php
$name = "Martin";
$age = 20;

echo "<h3> Hi! my name is " . $name . "</h3>";
echo "<h3> I am " . $age . " years old</h3>"

echo "<h3>" . $name . " is " . $age . " years old </h3>"
```

When concatenating strings with other data types, PHP automatically converts the other data types into their string equivalents.

For example: 
```php
$number = 12;
$result = "Answer " . $number;

echo $result;  // Answer 12
echo gettype($number); // integer
```
- The integer `12` is automatically converted into the string `"12"` during concatenation. 
- It does not change the original variable's data type. PHP only converts the value into a string temporarily for the concatenation process. The original variable retains its original data type.

Even though `$number` was converted into a string when concatenated with `"Answer "`, the original `$number` variable is still an integer. 

In simple terms:

- `$number` remains an integer (`12`).
- `$result` becomes a string (`"Answer 12"`).

Concatenation does not permanently change the original variable's data type.

## Easier way to Concatenate 

We can concatenate variables directly inside the double quotes

```php
$name = "Martin";
echo "Hi, $name";
```

```php
$name = "Martin";
$age = 20;

echo "<h3> Hi my name is $name </h3>";
echo "<h3> $name is $age years old </h3>";
```


- Note: Make sure to use double quotes `" "` instead of single quotes `' '`

___


