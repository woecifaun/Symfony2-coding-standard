# Symfony2 PHP CodeSniffer Coding Standard

A code standard to check against the [Symfony coding standards](http://symfony.com/doc/current/contributing/code/standards.html), forked from [opensky/Symfony2-coding-standard](https://github.com/opensky/Symfony2-coding-standard) to allow installation with composer.

The reason of the fork is to use this PHP CodeSniffer coding standard with [M6Web/Coke](https://github.com/M6Web/Coke).

http://tech.m6web.fr/verifier-la-coherence-du-code-d-un-projet-symfony2-avec-coke/ (in french)

## Installation

1. [Install composer](https://getcomposer.org/download/)
2. Create a composer.json file who contain:

    ```json
    {
        "require-dev": {
            "m6web/coke": "~1.1",
            "m6web/Symfony2-coding-standard": "~1.1"
        }
    }
    ```

3. Install dev dependencies

    ```shell
    composer update --dev
    ```

4. Create a `.coke` file a the root of the project who contain: 

    ```shell
    standard=vendor/m6web/symfony2-coding-standard/Symfony2
    ```

5. Enjoy

    ```shell
    ./vendor/bin/coke
    ```

## Credits

Developped by [M6Web](http://tech.m6web.fr/).

## License

This project is licensed under the [MIT license](LICENSE).
