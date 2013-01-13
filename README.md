JSON-js Bundle for Symfony2
=======================

## Current Version

JSON-js 2012-10-08
Only the json2.js file crockford is suggesting to use is included

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "bmatzner/json2-bundle": "*"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Bmatzner\Json2Bundle\BmatznerJson2Bundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update bmatzner/json2-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
<script type="text/javascript" src="{{ asset('bundles/bmatznerjson2/js/json2.min.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. https://github.com/douglascrockford/JSON-js
2. http://symfony.com
