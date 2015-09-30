# docker-php-5.3-cli
Build of 5.3 in the same style as the official PHP repository

Available on [Docker Hub](https://hub.docker.com/r/tomsowerby/php-5.3/)

We have some legacy projects that need to be build in an old PHP 5.3 environment.

This docker image is intended to allow composer and other build tools to be run on it to emulate dependancies on the production environment.

Thanks to [helderco](https://github.com/helderco/docker-php-5.3) for solving the openssl headache

The rest of this repo is borrowed from the [Official PHP image](https://github.com/docker-library/php) that no longer supports 5.3

Usage should be the same as the [Official PHP cli](https://hub.docker.com/_/php/)

Check the version:

	docker run -it --rm tomsowerby/php-5.3:cli php -v

Run a script:

	docker run -it --rm --name my-running-script -v "$PWD":/usr/src/myapp -w /usr/src/myapp tomsowerby/php-5.3:cli php your-script.php


Please report bugs for this container to the [GitHub issue](https://github.com/tomsowerby/docker-php-5.3-cli/issues) page.