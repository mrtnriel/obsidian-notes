1. Strings
2. String Length
3. String Indices
4. String Methods

___

# Strings 

One of the data types in PHP. It may be a character, word or sentence surrounded by `" "` or `' '`.  They are used to display text information.

## String Length

`strlen` is a function that gives the number of characters in a string

```php
<?php
	$name = "Martin";
	echo strlen($name); // Output: 6
?>
```

## String Indices

Individual characters can be accessed by using an index

```php
$name = "Martin";
```


| Elements | M   | a   | r   | t   | i   | n   |
| -------- | --- | --- | --- | --- | --- | --- |
| Index    | 0   | 1   | 2   | 3   | 4   | 5   |
We use `[]` square brackets to access the indices of a string

```php
$name = "Martin";
echo $name[0]; // Output: M
```

## String Methods

These different methods can manipulate strings in different ways

| Method         | Usage               | Description               |
| -------------- | ------------------- | ------------------------- |
| `strtoupper()` | `strtoupper($str)`  | Turns string to uppercase |
| `strtolower()` | `strtolower($str);` | Turns string to lowercase |
```php 
$name = "Martin";
$name = strtoupper($name);
echo $name; // Output: MARTIN
```


