# Hytale API - PHP SDK

Created by [mTxServ](https://mtxserv.com) and [Hytale.game](https://hytale.game).
With this SDK, you can consume the official Hytale API in PHP.

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/mTxServ/hytale-api-sdk-php.git"
    }
  ],
  "require": {
    "/": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
require_once(__DIR__ . '/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$year = 56; // int | Year (ex: 2019)
$month = 56; // int | Month (ex: 01)

try {
    $apiInstance->blogPostArchiveYearMonthGet($year, $month);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->blogPostArchiveYearMonthGet: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *http://hytale.com/api*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DefaultApi* | [**blogPostArchiveYearMonthGet**](docs/Api/DefaultApi.md#blogpostarchiveyearmonthget) | **GET** /blog/post/archive/{year}/{month}/ | 
*DefaultApi* | [**blogPostPublishedGet**](docs/Api/DefaultApi.md#blogpostpublishedget) | **GET** /blog/post/published | 
*DefaultApi* | [**blogPostSlugSlugGet**](docs/Api/DefaultApi.md#blogpostslugslugget) | **GET** /blog/post/slug/{slug} | 
*DefaultApi* | [**jobListingGet**](docs/Api/DefaultApi.md#joblistingget) | **GET** /job/listing | 


## Documentation For Authorization

 All endpoints do not require authorization.
