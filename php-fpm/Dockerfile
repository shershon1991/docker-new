FROM shershon/php-fpm:1.0
LABEL maintainer="Shershon <18810877074@163.com>"

# 时区
ARG TZ=UTC
ENV TZ ${TZ}
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

# 安装openVPN
RUN apt-get update && apt-get install -y openvpn

# 配置同步
#COPY  ./laravel.ini /usr/local/etc/php/conf.d
#COPY  ./opcache.ini /usr/local/etc/php/conf.d
#COPY  ./xdebug.ini /usr/local/etc/php/conf.d/xdebug.ini
#COPY  ./xlaravel.pool.conf /usr/local/etc/php-fpm.d/

WORKDIR /var/www
