# PoP GraphiQL

<!--
[![Latest Version on Packagist][ico-version]][link-packagist]
[![Software License][ico-license]](LICENSE.md)
[![Build Status][ico-travis]][link-travis]
[![Coverage Status][ico-scrutinizer]][link-scrutinizer]
[![Quality Score][ico-code-quality]][link-code-quality]
[![Total Downloads][ico-downloads]][link-downloads]
-->

Integrate the GraphiQL client on the PoP API Demo site

## Install

Via Composer

``` bash
$ composer require leoloso/pop-graphiql dev-master
```

**Note:** Your `composer.json` file must have the configuration below to accept minimum stability `"dev"` (there are no releases for PoP yet, and the code is installed directly from the `master` branch):

```javascript
{
    ...
    "minimum-stability": "dev",
    "prefer-stable": true,
    ...
}
```

In order to copy the GraphiQL under a specific path, install package [Composer Installers Extender](https://github.com/oomphinc/composer-installers-extender):

``` bash
$ composer require oomphinc/composer-installers-extender
```

Then, add the path in section `"extra"."installer-paths"`. For instance, this configuration will add the GraphiQL client under URL `/graphiql/`:

``` javascript
{
    ...
    "extra": {
        "installer-paths": {
            "graphiql/": [
                "leoloso/pop-graphiql"
            ]
        }
    }
}
```

<!--
## Usage

``` php
```
-->

## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Testing

``` bash
$ composer test
```

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) and [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md) for details.

## Security

If you discover any security related issues, please email leo@getpop.org instead of using the issue tracker.

## Credits

- [Leonardo Losoviz][link-author]
- [All Contributors][link-contributors]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[ico-version]: https://img.shields.io/packagist/v/getpop/event-mutations-wp-em.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/getpop/event-mutations-wp-em/master.svg?style=flat-square
[ico-scrutinizer]: https://img.shields.io/scrutinizer/coverage/g/getpop/event-mutations-wp-em.svg?style=flat-square
[ico-code-quality]: https://img.shields.io/scrutinizer/g/getpop/event-mutations-wp-em.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt/getpop/event-mutations-wp-em.svg?style=flat-square

[link-packagist]: https://packagist.org/packages/getpop/event-mutations-wp-em
[link-travis]: https://travis-ci.org/getpop/event-mutations-wp-em
[link-scrutinizer]: https://scrutinizer-ci.com/g/getpop/event-mutations-wp-em/code-structure
[link-code-quality]: https://scrutinizer-ci.com/g/getpop/event-mutations-wp-em
[link-downloads]: https://packagist.org/packages/getpop/event-mutations-wp-em
[link-author]: https://github.com/leoloso
[link-contributors]: ../../contributors
