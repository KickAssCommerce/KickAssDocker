# KickAssCommerce Docker

[![Latest Version on GitHub][ico-version]][link-release]
[![Software License][ico-license]](LICENSE.md)
[![Build Status][ico-travis]][link-travis]
[![Total Downloads][ico-downloads]][link-downloads]

## Quick Start

    mkdir kickass
    
    docker-compose run cli kickass-installer
    docker-compose up -d
    docker-compose restart
    
## Configuration

* `APP_ROOT` - The directory KickAssCommerce should be installed to (defaults to /var/www/kickass)
* `PHP_MEMORY_LIMIT` - The PHP memory limit to set in `php.ini`
* `PHP_ENABLE_XDEBUG` - Enable Xdebug

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) and [CONDUCT](CONDUCT.md) for details.

## Credits

Thanks to [Meanbee](https://github.com/meanbee) for their work on [docker-magento2](https://github.com/meanbee/docker-magento2) which has been used as the basis for this implementation.

- [KickAssCommerce Team][link-author]
- [All Contributors][link-contributors]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[ico-version]: https://img.shields.io/github/release/KickAssCommerce/KickAssDocker.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/KickAssCommerce/KickAssDocker/develop.svg?style=flat-square
[ico-downloads]: https://img.shields.io/docker/pulls/kickasscommerce/kickasscommerce.svg?style=flat-square

[link-release]: https://github.com/KickAssCommerce/KickAssDocker/releases
[link-travis]: https://travis-ci.org/KickAssCommerce/KickAssDocker
[link-author]: https://github.com/kickasscommerce
[link-downloads]: https://hub.docker.com/r/kickasscommerce/kickasscommerce/
[link-contributors]: ../../contributors