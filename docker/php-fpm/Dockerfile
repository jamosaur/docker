FROM phpdockerio/php71-fpm:latest

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install php7.1-dev php7.1-mbstring php7.1-curl php7.1-mcrypt php7.1-gd php7.1-xdebug php7.1-mysql php7.1-gmp php7.1-zip php7.1-dom php-xml php-imagick php-ssh2 php-xdebug git \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*


WORKDIR "/application"
