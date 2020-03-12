# This project is abandoned

This repo is being kept for posterity and will be archived in a readonly state. 
If you're interested it can be forked under a new Composer namespace/GitHub organization.

# phergie/phergie-irc-plugin-react-commandalias

[Phergie](http://github.com/phergie/phergie-irc-bot-react/) plugin for enabling the use of custom aliases for existing bot commands.

This plugin is intended to complement the [Command plugin](https://github.com/phergie/phergie-irc-plugin-react-command).

[![Build Status](https://secure.travis-ci.org/phergie/phergie-irc-plugin-react-commandalias.png?branch=master)](http://travis-ci.org/phergie/phergie-irc-plugin-react-commandalias)

## Install

The recommended method of installation is [through composer](http://getcomposer.org).

```JSON
{
    "require": {
        "phergie/phergie-irc-plugin-react-commandalias": "dev-master"
    }
}
```

See Phergie documentation for more information on
[installing and enabling plugins](https://github.com/phergie/phergie-irc-bot-react/wiki/Usage#plugins).

## Configuration

```php
new \Phergie\Irc\Plugin\React\CommandAlias\Plugin(array(

    // All configuration is required

    'aliases' => array(
        // alias => command
        'j' => 'join',
        'p' => 'part',
        'q' => 'quit',
        'btc' => 'wolfram-alpha 1 BTC in US$',
        // ...
    ),

))
```

## Tests

To run the unit test suite:

```
curl -s https://getcomposer.org/installer | php
php composer.phar install
./vendor/bin/phpunit
```

## License

Released under the BSD License. See `LICENSE`.
