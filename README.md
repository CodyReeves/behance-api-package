Behance API -- Development in Progress 
=======

Behance API Package for Laravel 5.3

## Installation

Install this package through Composer. Edit your project's `composer.json`, Add this below:
  
  
 ```
 "require": {
    "codyreeves/behance": "dev-master"
  }
 ```
  
  
 ```
 "repositories": [
    {
        "type": "vcs"
    	"url": "https://github.com/CodyReeves/behance-api-package"
    }
  ]
```

Update Composer:

    composer update

Add the service provider. Open `app/config/app.php`, and add a new item to the Aliases array.

    'Behance' => CodyReeves\Behance\BehanceServiceProvider::class,


## Usage

Example of how to get the featured projects:

```php
print_r(Behance::searchProjects());
```

Info on using the Behance API: https://github.com/behance/network_api_php
