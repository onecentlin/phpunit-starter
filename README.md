# PHPUnit Starter

## Prerequisite

1. PHP 7.1 (https://php.net/downloads.php)
2. Composer (https://getcomposer.org/)
3. PHPUnit 7.1 (https://phpunit.de/)

For command line use, please setup properly for global environment.

## Installation

Install phpunit for project

    composer install

## Folder Structures

```
Project/
    |-- src/    (php source code)
    |-- tests/  (Testing files)
    |-- composer.json   (Composer configuration file)
    |-- phpunit.xml     (PHPUnit configuration file)
```

## Run PHPUnit in Terminal

Run all testing files in `tests/` folder

```bash
vendor/bin/phpunit tests
```

Run testing settings in phpunit.xml configuration

```bash
vendor/bin/phpunit
```

## Basic PHP Test File

1. Class with `Test` for naming convention.
2. Test Class MUST extends `PHPUnit\Framework\TestCase`
3. Method name starts with `test` or with annotation `/** @test */`
4. Name file with suffix `Test.php`.

Example: `ExampleTest.php`

```php
<?php

use PHPUnit\Framework\TestCase;

class ExampleTest extends TestCase
{
    /** @test */
    public function test_feature()
    {
        // arrange
        
        // act
        
        // assert

    }
}
```

- PHPUnit Assertions (https://phpunit.de/manual/current/en/appendixes.assertions.html)
- PHPUnit Configration (http://phpunit.readthedocs.io/en/7.1/configuration.html)
- Visit [PHPUnit Manual](https://phpunit.de/manual/current/en/) for more information.
