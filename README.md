Yii2 sphinx api
===============
Yii2 sphinx api

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist schevgeny/sphinx "*"
```

or add

```
"schevgeny/sphinx": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Add component sphinx to config  :
```php
'components' => [
    ...
    'sphinx' => [
        'class' => 'schevgeny\sphinx\DGSphinxSearch',
        'server' => 'SPHINX_SERVER_IP',
        'port' => 3312,
        'maxQueryTime' => 3000,
        'enableProfiling'=>0,
        'enableResultTrace'=>0,
        'fieldWeights' => [
            'name' => 10000,
            'keywords' => 100,
        ],
    ],
]
