## Status

[![Build Status](https://travis-ci.org/zeuxisoo/php-slim-whoops.png?branch=master)](https://travis-ci.org/zeuxisoo/php-slim-whoops)

## Installing

- Install the composer

```
curl -sS https://getcomposer.org/installer | php
```

- Edit composer.json

```
{
	"require": {
		"zeuxisoo/slim-whoops": "dev-master"
	}
}
```

- Install/update your dependencies

```
php composer.phar install
```

## Usage

- add the middleware into slim application

```
$app->add(new \Zeuxisoo\Whoops\Provider\Slim\WhoopsMiddleware);
```

## Options

- Opening referenced files with your favorite editor or IDE

```
$app->config('whoops.editor', 'sublime');  // add this line
$app->add(new \Zeuxisoo\Whoops\Provider\Slim\WhoopsMiddleware);
```

## Important Note

- Please make sure you already installed **whoops** library.

## Testing

- Run the test cases

```
php vendor/bin/phpunit
```
