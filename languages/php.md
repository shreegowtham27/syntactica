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




