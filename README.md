yii2-assetConverter
=========

Yii2 assets compiler
Currently support less


change less compiler "leafo/lessphp" to "oyejorge/less.php" for support bootstrap less

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist singrana/yii2-assetConverter "*"
```

or add

```
"singrana/yii2-assetConverter": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Add or modify your Yii2 application config


```php
'components'    =>
[
	'assetManager'					=>
	[
		'converter'					=>
		[
			'class'					=>	'singrana\assetConverter\Converter',
		],
	...
	],
	...
];
```

after this, you can usage in you bundles, for example:

```php

	public $css =
	[
		'css/style.less',
	];
```