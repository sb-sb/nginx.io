# Nginx.io

> Advanced Nginx Debian / Ubuntu repository

## What it is

The default nginx repository from official Debian or Ubuntu image is always out-of-date, so we build nginx.io and you can install the latest nginx simply via `apt install nginx-extras`

Nginx.io is based on official [Debian Nginx packaging repository](https://salsa.debian.org/nginx-team/nginx)

## Current Version

Nginx / 1.17.8

## Features

Everything from nginx-extras included, and we also add these nginx modules

* [ngx_http_geoip2_module](https://github.com/leev/ngx_http_geoip2_module)
* [ngx_brotli](https://github.com/google/ngx_brotli)
* [ngx_http_ipdb_module](https://github.com/vislee/ngx_http_ipdb_module)

Built with OpenSSL 1.1.1d, you can use TLS 1.3 on SSL configuration.

Sample output:

```
root@server ~ # nginx -V
nginx version: nginx/1.17.8
built with OpenSSL 1.1.1d  10 Sep 2019
TLS SNI support enabled
configure arguments: --with-cc-opt='-g -O2 -fdebug-prefix-map=/build/nginx=. -fstack-protector-strong -Wformat -Werror=format-security -fPIC -Wdate-time -D_FORTIFY_SOURCE=2' --with-ld-opt='-Wl,-z,relro -Wl,-z,now -fPIC' --with-openssl=/build/nginx/../openssl --prefix=/usr/share/nginx --conf-path=/etc/nginx/nginx.conf --http-log-path=/var/log/nginx/access.log --error-log-path=/var/log/nginx/error.log --lock-path=/var/lock/nginx.lock --pid-path=/run/nginx.pid --modules-path=/usr/lib/nginx/modules --http-client-body-temp-path=/var/lib/nginx/body --http-fastcgi-temp-path=/var/lib/nginx/fastcgi --http-proxy-temp-path=/var/lib/nginx/proxy --http-scgi-temp-path=/var/lib/nginx/scgi --http-uwsgi-temp-path=/var/lib/nginx/uwsgi --with-debug --with-pcre-jit --with-http_ssl_module --with-http_stub_status_module --with-http_realip_module --with-http_auth_request_module --with-http_v2_module --with-http_dav_module --with-http_slice_module --with-threads --with-http_addition_module --with-http_flv_module --with-http_geoip_module=dynamic --with-http_gunzip_module --with-http_gzip_static_module --with-http_image_filter_module=dynamic --with-http_mp4_module --with-http_perl_module=dynamic --with-http_random_index_module --with-http_secure_link_module --with-http_sub_module --with-http_xslt_module=dynamic --with-mail=dynamic --with-mail_ssl_module --with-stream=dynamic --with-stream_ssl_module --with-stream_ssl_preread_module --add-dynamic-module=/build/nginx/sb-modules/ngx_http_geoip2_module --add-dynamic-module=/build/nginx/sb-modules/ngx_http_ipdb_module --add-module=/build/nginx/sb-modules/ngx_brotli --add-dynamic-module=/build/nginx/debian/modules/http-headers-more-filter --add-dynamic-module=/build/nginx/debian/modules/http-auth-pam --add-dynamic-module=/build/nginx/debian/modules/http-cache-purge --add-dynamic-module=/build/nginx/debian/modules/http-dav-ext --add-dynamic-module=/build/nginx/debian/modules/http-ndk --add-dynamic-module=/build/nginx/debian/modules/http-echo --add-dynamic-module=/build/nginx/debian/modules/http-fancyindex --add-dynamic-module=/build/nginx/debian/modules/nchan --add-dynamic-module=/build/nginx/debian/modules/http-lua --add-dynamic-module=/build/nginx/debian/modules/rtmp --add-dynamic-module=/build/nginx/debian/modules/http-uploadprogress --add-dynamic-module=/build/nginx/debian/modules/http-upstream-fair --add-dynamic-module=/build/nginx/debian/modules/http-subs-filter
```