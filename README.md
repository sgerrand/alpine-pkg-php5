# alpine-pkg-php5

[![CircleCI](https://img.shields.io/circleci/project/sgerrand/alpine-pkg-php5/master.svg)](https://circleci.com/gh/sgerrand/alpine-pkg-php5)

This is the [PHP 5][php] language runtime engine as an Alpine Linux package. It includes a patch for a [NaN bug][php-nan-bug] with [musl libc][musl].

## Releases

See the [releases page](https://github.com/sgerrand/alpine-pkg-php5/releases) for the latest
download links.

## Installing

The current installation method for these packages is to pull them in using
`wget` or `curl` and install the local file with `apk`:

    apk --no-cache add ca-certificates wget
    wget -q -O /etc/apk/keys/sgerrand.rsa.pub https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub
    wget https://github.com/sgerrand/alpine-pkg-php5/releases/download/5.6.36-r1/php5-5.6.36-r1.apk
    apk add --no-cache php5-5.6.36-r1.apk

[musl]: http://www.musl-libc.org/
[php-nan-bug]: https://bugs.php.net/bug.php?id=73954
[php]: https://php.net
