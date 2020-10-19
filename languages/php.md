# PHP Cheat Sheet

## variable 

Variables in PHP are represented by a dollar sign followed by the name of the variable. The variable name is case-sensitive.
Variable names follow the same rules as other labels in PHP. A valid variable name starts with a letter or underscore, followed by any number of letters, numbers, or underscores.

example 

```
<?php
$var = 'Bob';
$Var = 'Joe';
echo "$var, $Var";      // outputs "Bob, Joe"

$4site = 'not yet';     // invalid; starts with a number
$_4site = 'not yet';    // valid; starts with an underscore
$täyte = 'mansikka';    // valid; 'ä' is (Extended) ASCII 228.
?>
```

## Data Types

PHP supports ten primitive types.

Four scalar types:

- boolean
- integer
- float (floating-point number, aka double)
- string

Four compound types:

- array
- object
- callable
- iterable

And finally two special types:

- resource
- NULL


## Check a Valid Data

**boolval** — Used to retrieve the boolean value of a variable

**debug_zval_dump** — Outputs a string representation of an internal zend value

**empty** — Checks whether a variable is empty or not

**floatval** — Get the float value of a variable (doubleval is another possibility)

**get_defined_vars** — Returns an array of all defined variables

**get_resource_type** — Returns the resource type

**gettype** — Retrieves the variable type

**import_request_variables** — Import GET/POST/Cookie variables into the global scope

**intval** — Find the integer value of a variable

**is_array** — Checks whether a variable is an array

**is_bool** — Finds out if a variable is a boolean

**is_callable** — Verify whether you can call the contents of a variable as a function

**is_countable** — Check whether the contents of a variable are countable

**is_float** — Find out if the type of a variable is float, alternatives: is_double and is_real

**is_int** — Check if the type of a variable is an integer, is_integer and is_long also works

**is_iterable** — Verify that a variable’s content is an iterable value

**is_null** — Checks whether a variable’s value is NULL

**is_numeric** — Find out if a variable is a number or a numeric string

**is_object** — Determines whether a variable is an object

**is_resource** — Check if a variable is a resource

**is_scalar** — Tests if a variable is a scalar

**is_string** — Find out whether the type of a variable is a string

**isset** — Determine if a variable has been set and is not NULL

**print_r** — Provides human-readable information about a variable

**serialize** — Generates a representation of a value that is storable

**settype** — Sets a variable’s type

**strval** — Retrieves the string value of a variable

**unserialize** — Creates a PHP value from a stored representation

**unset** — Unsets a variable

**var_dump** — Dumps information about a variable

**var_export** — Outputs or returns a string representation of a variable that can be parsed


### PHP Operators

Operators are used to perform certain operations on variables or values or sometimes both the values and Variables.

#### PHP Operator Types:

- Arithmetic operators
- Assignment operators
- Comparison operators
- Increment/Decrement operators
- Logical operators
- String operators
- Array operators
- Conditional assignment operators

#### PHP Arithmetic Operators

Arithmetic operators are used to perform common arithmetical operations, such as addition, subtraction, multiplication etc., between any two or more numberic data types.


| Operator 	   |    Name 	       | Example    |   Result	                                |
|--------------|-------------------|------------|-------------------------------------------|
| + 	       | Addition 	       | $x + $y 	|   Adds Two Variables 	                    |
| - 	       | Subtraction 	   | $x - $y 	|   Subtracts $x from $y 	                |
| * 	       | Multiplication    | $x * $y 	|   Product of $x and $y 	                |
| / 	       | Division 	       | $x / $y 	|   Quotient of $x and $y 	                |
| % 	       | Modulus 	       | $x % $y 	|   Remainder of $x when divided by $y 	    |
| ** 	       | Exponentiation    | $x ** $y 	|   Result of raising $x to the $y'th power |


#### PHP Assignment Operators

The PHP assignment operators are used with numeric values to write a value to a variable.

The basic assignment operator in PHP is "=". It means that the left operand gets set to the value of the assignment expression on the right.

|   Assignment |  Similar/same to  |    Description                                                              |
|--------------|-------------------|-----------------------------------------------------------------------------|
|   x = y 	   |    x = y 	       |     The left operand gets set to the value of the expression on the right 	 |
|   x += y 	   |    x = x + y 	   |     Addition 	                                                             |
|   x -= y 	   |    x = x - y 	   |     Subtraction 	                                                         |
|   x *= y 	   |    x = x * y 	   |     Multiplication 	                                                     |
|   x /= y 	   |    x = x / y 	   |     Division 	                                                             |
|   x %= y 	   |    x = x % y 	   |     Modulus 	                                                             |



#### PHP Comparison Operators

The PHP comparison operators are used to compare two values (number or string):

| Operator 	   |     Name 	              | Example 	|       Result 	                                                             |
|--------------|--------------------------|-------------|----------------------------------------------------------------------------|
| == 	       | Equal                    | $x == $y 	|   Returns true if $x is equal to $y 	                                     |
| === 	       | Identical 	              | $x === $y 	|   Returns true if $x is equal to $y, and they are of the same type 	     |
| != 	       | Not equal 	              | $x != $y 	|   Returns true if $x is not equal to $y 	                                 |
| <> 	       | Not equal 	              | $x <> $y 	|   Returns true if $x is not equal to $y 	                                 |
| !== 	       | Not identical 	          | $x !== $y 	|   Returns true if $x is not equal to $y, or they are not of the same type  |
| > 	       | Greater than 	          | $x > $y 	|   Returns true if $x is greater than $y 	                                 |
| < 	       | Less than 	              | $x < $y 	|   Returns true if $x is less than $y 	                                     |
| >= 	       | Greater than or equal to |	$x >= $y 	|   Returns true if $x is greater than or equal to $y 	                     |
| <= 	       | Less than or equal to 	  | $x <= $y 	|   Returns true if $x is less than or equal to $y 	                         |
| <=> 	       | Spaceship 	              | $x <=> $y 	|   Returns an integer less than, equal to, or greater than zero,            |  
|              |                          |             |   depending on if $x is less than, equal to, or greater than $y.           | 
|              |                          |             |   **Introduced in PHP 7.**                                                 |
