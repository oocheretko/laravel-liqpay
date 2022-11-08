# Laravel LiqPay
A Laravel package for the LiqPay PHP SDK.
Fork and change dependencies deniztezcan/laravel-liqpay
## Instalation
```
composer require ocheretko/laravel-liqpay
```

Add a ServiceProvider to your providers array in `config/app.php`:
```php
    'providers' => [
    	//other things here

    	DenizTezcan\LiqPay\LiqPayServiceProvider::class,
    ];
```

Add the facade to the facades array:
```php
    'aliases' => [
    	//other things here

    	'LiqPay' => DenizTezcan\LiqPay\Facades\LiqPay::class,
    ];
```

Finally, publish the configuration files:
```
php artisan vendor:publish --provider="DenizTezcan\LiqPay\LiqPayServiceProvider"
```

### Configuration
Please set your API: `LIQPAY_PUBLIC` and `LIQPAY_PRIVATE` in the `.env` file 