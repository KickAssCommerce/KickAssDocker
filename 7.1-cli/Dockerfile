# FPM, PHP 7.1, KickAssCommerce compatible container.

FROM php:7.1-cli

MAINTAINER Adam Paterson <hello@adampaterson.co.uk>

# Install PHP extension dependancies
RUN apt-get update \
  && apt-get install -y \
    libicu-dev \
    libmcrypt-dev \
    libxslt1-dev \
    zlib1g-dev \
    git

# Install required PHP extensions
RUN docker-php-ext-install \
  intl \
  mbstring \
  mcrypt \
  xsl \
  zip \
  soap

# Install PHP7 compatible version of xdebug
RUN pecl install -o -f xdebug-2.5.0

# Install composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Define volume for caching composer packages
VOLUME /root/.composer/cache

# Add executables and config
ADD bin/* /usr/local/bin/
ADD etc/php.ini /usr/local/etc/php/conf.d/zz-kickass.ini
ADD etc/php-xdebug.ini /usr/local/etc/php/conf.d/zz-xdebug.ini

# Define default environment variables
ENV PHP_MEMORY_LIMIT 2G
ENV PHP_ENABLE_XDEBUG false
ENV APP_ROOT /var/www/kickass

ENTRYPOINT ["/usr/local/bin/docker-environment"]
CMD ["bash"]