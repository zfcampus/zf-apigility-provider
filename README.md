ZF Apigility Provider
=====================

> ## Repository abandoned 2019-12-31
>
> This repository has moved to laminas-api-tools/api-tools-provider.

[![Build Status](https://secure.travis-ci.org/zfcampus/zf-apigility-provider.svg?branch=master)](https://secure.travis-ci.org/zfcampus/zf-apigility-provider)

Introduction
------------

This repository consists of interfaces used by Apigility that can be composed
into standalone modules and libraries so that consumers may choose to opt-in to
Apigility functionality.

### General Usage

To mark a module as being an Apigility-enabled module, add the following
interface to your Module:

```php
use ZF\Apigility\Provider\ApigilityProviderInterface;

class MyModule implements ApigilityProviderInterface
{
}
```

At this point, this particular module should show up in the Apigility UI interface.

Requirements
------------
  
Please see the [composer.json](composer.json) file.

Installation
------------

Run the following `composer` command:

```console
$ composer require zfcampus/zf-apigility-provider
```

Alternately, manually add the following to your `composer.json`, in the `require` section:

```javascript
"require": {
    "zfcampus/zf-apigility-provider": "^1.0"
}
```

And then run `composer update` to ensure the module is installed.