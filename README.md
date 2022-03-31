# Helper Function Example in Laravel 8

We will see helper function example in laravel, Laravel provide in-buit global "helper" PHP functions and these functions are used by the laravel framework itself.

Here i will show laravel 8 global helper function with differnt type of example and also we will see how to use global helper function in laravel 8.

 

Exmaple : 

bcrypt() :  This function through you can convert your password into bcrypt.
```php
$pwd = bcrypt('password');
```
cookie() : The cookie function creates a new cookie instance.
```php
$cookie = cookie('name', 'value', $minutes);
```

 csrf_field():This function generates an HTML hidden input field containing the value of the CSRF token.
```php
{{ csrf_field() }}
```

csrf_token(): This function retrieves the value of the current CSRF token.
```php
$token = csrf_token();
``` 

dd():  This function dumps the given variables and ends execution of the script.
```php
dd($value);
``` 

now () : This function return current time.
```php
$time = now();
``` 

Str::between : This method returns the part of a string between two values. if we need to use str function then we need to add Illuminate\Support\Str class.
```php
use Illuminate\Support\Str;

$slice = Str::between('This is demo example', 'This', 'example');

// it will return ' is demo '
``` 

Str::camel : This method converts string into camelcase.
```php
use Illuminate\Support\Str;

$example = Str::camel('hello_all');

// helloAll
``` 

Str::contains: This method check if the given string contains the given value, it is case sensitive.
```php
use Illuminate\Support\Str;

$contains = Str::contains('This is demo example', 'demo');

// true
``` 

Arr::random : This method returns a random value from an array if we need to use str function then we need to add use Illuminate\Support\Arr  class.
```php
use Illuminate\Support\Arr;

$array = [1, 2, 3, 4, 5];

$random = Arr::random($array);

// 2 - it will return random number
```
