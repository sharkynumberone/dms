FROM serkyron/apache2-nginx-php7.0

RUN apt-get update && apt-get install -y \
    python-software-properties

RUN LC_ALL=C.UTF-8 add-apt-repository ppa:ondrej/php

RUN apt-get update && apt-get install -y \
    php7.2 \
    libapache2-mod-php7.2 \
	php7.2-cgi \
	php7.2-cli \
	php7.2-curl \
	php7.2-gd \
	php7.2-imap \
	php7.2-intl \
	php7.2-json \
	php7.2-ldap \
	php7.2-mbstring \
	php7.2-mysql \
	php7.2-opcache \
	php7.2-pspell \
	php7.2-readline \
	php7.2-soap \
	php7.2-xml

WORKDIR /var/www/
COPY entrypoint /usr/bin
ENTRYPOINT ["entrypoint"]
