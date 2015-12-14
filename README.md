# CKEditor Plugin Notification Bundle
Symfony2 Bundle to integrate the CKEditor plugin Aggregator

## Current Version

Notification v4.5.6

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/ckeditor-notification-bundle": "~4.5.6"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Stinger\CKEditorNotificationBundle\StingerCKEditorNotificationBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/ckeditor-notification-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

### Usage

``` yaml
trsteel_ckeditor:
    external_plugins:
      notification:
        path: 'bundles/stingerckeditornotification'
```



# Licenses

Refer to the source code of the included files for license information

# References

1. http://ckeditor.com/addon/notification
2. http://symfony.com
