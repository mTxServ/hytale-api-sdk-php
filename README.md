# Hytale API - PHP SDK

Created by [mTxServ](https://mtxserv.com) and [Hytale.game](https://hytale.game).
With this SDK, you can consume the official Hytale API in PHP.

![Travis (.org)](https://img.shields.io/travis/mTxServ/hytale-api-sdk-php.svg)

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
composer require hytale-game/hytale-api-sdk-php
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
    $result = $apiInstance->getArticles($featured_only);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ArticlesApi->getArticles: ', $e->getMessage(), PHP_EOL;
}
?>
```

## Documentation for API Endpoints

All URIs are relative to *http://hytale.com/api*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ArticlesApi* | [**getArticleBySlug**](docs/Api/ArticlesApi.md#getarticlebyslug) | **GET** /blog/post/slug/{slug} | 
*ArticlesApi* | [**getArticles**](docs/Api/ArticlesApi.md#getarticles) | **GET** /blog/post/published | 
*ArticlesApi* | [**getArticlesOfMonthAndYear**](docs/Api/ArticlesApi.md#getarticlesofmonthandyear) | **GET** /blog/post/archive/{year}/{month}/ | 
*JobsApi* | [**getJobs**](docs/Api/JobsApi.md#getjobs) | **GET** /job/listing | 


## Documentation For Models

 - [Article](docs/Model/Article.md)
 - [CoverImage](docs/Model/CoverImage.md)
 - [Job](docs/Model/Job.md)


## Documentation For Authorization

 All endpoints do not require authorization.