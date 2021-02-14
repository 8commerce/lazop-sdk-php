# 8Commerce 
[8Commerce](http://www.8commerce.com) is Indonesia ecommerce enabler, e-fulfillment and logistic service. Our focus is your
customer satisfaction by providing best online shopping experience.

# PHP Library for the Lazada Open API
Usage of this library is also available at [Lazada Open API](https://open.lazada.com)

Requirements
-----

PHP SDK requires PHP 5 or newer version

Composer Installation
-----

Run the following command:
```bash
composer require 8commerce/lazop-sdk-php
```

Usage
-----

Sample usage:
```php
use 8commerce\PHPLazadaSDK\LazopClient;
use 8commerce\PHPLazadaSDK\LazopRequest;

...
$c = new LazopClient('https://api.lazada.test/rest', '${appKey}', '${appSecret}');
$request = new LazopRequest('/mock/api/get');
$request->addApiParam('api_id',1);
$request->addHttpHeaderParam('cx','test');
    
var_dump($c->execute($request));
...

```