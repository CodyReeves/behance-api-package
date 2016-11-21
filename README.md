Behance API -- Development in Progress 
=======

Behance API Package for Laravel 5.3

## Installation

Install this package through Composer. Edit your project's `composer.json` Add one of the two below:
  
  -- Not an available method  of installation -- Method addintion TBA 
  
 ` "require": {
    "codyreeves/behance": "dev-master"
  }`
  
  or 
  
  `"repositories": [
    {
        "type": "vcs",
    	"url": "https://github.com/CodyReeves/behance-api-package"
    }
  ]`

Update Composer:

    composer update

Add the service provider. Open `app/config/app.php`, and add a new item to the providers array.

    'CodyReeves\Behance\BehanceServiceProvider',

Publish the config file. Enter the following command in Terminal.

    php artisan config:publish codyreeves/behance

Lastly, open `app/config/packages/codyreeves/behance/keys.php` and add your Behance Client ID and Client Secret.

## Usage

Example of how to get the featured projects:

```php
print_r(Behance::searchProjects());
```

Info on using the Behance API: https://github.com/behance/network_api_php
