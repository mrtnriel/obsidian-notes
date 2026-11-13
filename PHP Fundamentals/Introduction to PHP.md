___
# PHP 
PHP (HyperText Preprocessor) is a server-side programming language for websites (Backend)

It can generate dynamic page content based on logical checks and can connect to databases and perform complex data management

# Local Web Server

Are used to run server-side languages such as PHP, it provides a development server that can be accessed through the localhost and an open port.

- WAMP (Windows, Apache,  MySQL, PHP)
- MAMP (MacOS, Apache,  MySQL, PHP)
- XAMPP (Cross-Platform, Apache, MySQL, Perl, PHP)

# PHP Files

PHP Files are used instead of HTML files when creating a PHP Based website

PHP Files are saved with the extension: `.php`

- PHP Files can contain HTML, CSS & JSS

It is ideal to name your first PHP file into `index.php` so that the local server automatically makes it the root URL 

# PHP Script

It can be placed in any part of the document (head, body or even outside of the html tags)

```php
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Example PHP</title>
</head>
<body>
	<?php // Code goes here // ?>
</body>
</html>
```

- PHP Snippers starts with `<?php` and ends with `?>`

## Echo 

Use `echo` to display something as an HTML element of Text

```php
<?php echo "Hello World"; ?>
```
```php
<?php echo "<h1>Hello World</h1>"; ?>
```
```php
<?php echo "<input type='date'/>"; ?>
```
```php
<?php echo "<script> alert('Hi'); </script>"; ?>
```

- `echo` can be used to display elements by typing the intended tag name

	- Note: In PHP, Semicolon is required

When using multiple echo make sure to use `<br>` to separate lines

```php
echo "Hello";
echo "<br>";
echo "World";
```

We can also use `<p>` because it automatically puts the next element on a new line

```php
echo "<p>Hello</p>";
echo "<p>World</p>";
```