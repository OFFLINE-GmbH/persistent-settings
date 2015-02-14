# Persistent Settings Manager for Laravel 5
## Install it
To install this package include it in your `composer.json` and run `composer update`:

    "require": {
       "offline/persistent-settings": "dev-master"
    }
     
Add the Service Provider to the `provider` array in your `config/app.php`

    'Offline\Settings\SettingsServiceProvider'
    
Add an alias for the facade to your `config/app.php`

    'Settings'  => 'Offline\Settings\Facades\Settings',

Publish the config and migration files:

    $ php artisan vendor:publish --provider="Offline\Settings\SettingsServiceProvider"

## Use it