# KickAssCommerce Docker

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

[link-author]: https://github.com/kickasscommerce
[link-contributors]: ../../contributors