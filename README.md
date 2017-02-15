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

# Credits

Thanks to [Meanbee](https://github.com/meanbee) for their work on [docker-magento2](https://github.com/meanbee/docker-magento2) which has been used as the basis for this implementation.