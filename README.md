<a href="https://github.com/boson-php/boson">
    <img align="center" src="https://habrastorage.org/webt/-8/h1/5o/-8h15o6klbga13kzsltqqmk8jlm.png" />
</a>

---

<p align="center">
    <a href="https://packagist.org/packages/boson-php/symfony-bundle"><img src="https://poser.pugx.org/boson-php/symfony-bundle/require/php?style=for-the-badge" alt="PHP 8.4+"></a>
    <a href="https://packagist.org/packages/boson-php/symfony-bundle"><img src="https://poser.pugx.org/boson-php/symfony-bundle/version?style=for-the-badge" alt="Latest Stable Version"></a>
    <a href="https://packagist.org/packages/boson-php/symfony-bundle"><img src="https://poser.pugx.org/boson-php/symfony-bundle/v/unstable?style=for-the-badge" alt="Latest Unstable Version"></a>
    <a href="https://raw.githubusercontent.com/boson-php/boson/blob/master/LICENSE"><img src="https://poser.pugx.org/boson-php/symfony-bundle/license?style=for-the-badge" alt="License MIT"></a>
    <a href="https://t.me/boson_php"><img src="https://img.shields.io/static/v1?label=&message=Join+To+Community&color=24A1DE&style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram" /></a>
</p>
<p align="center">
    <a href="https://github.com/boson-php/symfony-bundle/actions/workflows/tests.yml"><img src="https://img.shields.io/github/actions/workflow/status/boson-php/boson/tests.yml?label=Tests&style=flat-square&logo=unpkg"></a>
</p>

## Installation

Boson package is available as Composer repository and can 
be installed using the following command in a root of your project:

```bash
composer require boson-php/symfony-bundle
```

- Add bundle into the registered `config/bundles.php` list:
```php
<?php

return [
    // ...
    Boson\Bridge\Symfony\BosonBundle::class => ['all' => true],
];
```

- Use the `APP_RUNTIME` environment variable or by specifying the 
  `extra.runtime.class` in `composer.json` to set the 
  [Runtime](https://symfony.com/doc/current/components/runtime.html) class:
```json
{
    "require": {
        "...": "..."
    },
    "extra": {
        "runtime": {
            "class": "Boson\\Bridge\\Symfony\\Runtime\\BosonRuntime"
        }
    }
}
```

- Initialize default configuration:
```php
php ./bin/console config:dump-reference boson > config/packages/boson.yaml
```

## Documentation

- You can learn more [about what a Boson is](https://bosonphp.com/doc/0.19/introduction).
- Information [about the configs](https://bosonphp.com/doc/0.19/configuration) is 
  available on the [corresponding pages](https://bosonphp.com/doc/0.19/application-configuration).
- A more detailed description of working with the [application](https://bosonphp.com/doc/0.19/application), 
  [windows](https://bosonphp.com/doc/0.19/window) and [webview](https://bosonphp.com/doc/0.19/webview) 
  is also available.
- Also, do not miss the detailed guide on additional apps for working with 
  [function bindings](https://bosonphp.com/doc/0.19/bindings-api),
  [scripts](https://bosonphp.com/doc/0.19/scripts-api),
  [request interception](https://bosonphp.com/doc/0.19/schemes-api), and more.
- If you want to build an application based on 
  [Symfony](https://bosonphp.com/doc/0.19/symfony-adapter), 
  [Laravel](https://bosonphp.com/doc/0.19/laravel-adapter) and 
  [others](https://bosonphp.com/doc/0.19/psr7-adapter), 
  then similar functionality is also available.

## Community

- Any questions left? You can ask them 
  [in the chat `t.me/boson_php`](https://t.me/boson_php)!

## Contributing

Boson is an Open Source, [community-driven project](https://github.com/boson-php/boson/graphs/contributors). 
Join them [contributing code](https://bosonphp.com/doc/0.19/contribution).

