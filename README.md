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
    "hytale-game/hytale-api-sdk-php": "*@dev"
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

$apiInstance = new Swagger\Client\Api\ArticlesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$featured_only = true; // bool | 

try {
    $result = $apiInstance->blogPostPublishedGet($featured_only);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ArticlesApi->blogPostPublishedGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

## Documentation for API Endpoints

All URIs are relative to *http://hytale.com/api*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ArticlesApi* | [**blogPostArchiveYearMonthGet**](docs/Api/ArticlesApi.md#blogpostarchiveyearmonthget) | **GET** /blog/post/archive/{year}/{month}/ | 
*ArticlesApi* | [**blogPostPublishedGet**](docs/Api/ArticlesApi.md#blogpostpublishedget) | **GET** /blog/post/published | 
*ArticlesApi* | [**blogPostSlugSlugGet**](docs/Api/ArticlesApi.md#blogpostslugslugget) | **GET** /blog/post/slug/{slug} | 
*JobsApi* | [**jobListingGet**](docs/Api/JobsApi.md#joblistingget) | **GET** /job/listing | 

## Documentation For Models

 - [Article](docs/Model/Article.md)
 - [CoverImage](docs/Model/CoverImage.md)
 - [Job](docs/Model/Job.md)


## Documentation For Authorization

 All endpoints do not require authorization.
