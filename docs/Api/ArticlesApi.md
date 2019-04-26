# Swagger\Client\ArticlesApi

All URIs are relative to *http://hytale.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**blogPostArchiveYearMonthGet**](ArticlesApi.md#blogPostArchiveYearMonthGet) | **GET** /blog/post/archive/{year}/{month}/ | 
[**blogPostPublishedGet**](ArticlesApi.md#blogPostPublishedGet) | **GET** /blog/post/published | 
[**blogPostSlugSlugGet**](ArticlesApi.md#blogPostSlugSlugGet) | **GET** /blog/post/slug/{slug} | 


# **blogPostArchiveYearMonthGet**
> \Swagger\Client\Model\Article[] blogPostArchiveYearMonthGet($year, $month)



Get list of articles published on a specific month of an year

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ArticlesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$year = 2019; // int | Year (ex: 2019)
$month = 01; // int | Month (ex: 01)

try {
    $result = $apiInstance->blogPostArchiveYearMonthGet($year, $month);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ArticlesApi->blogPostArchiveYearMonthGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **int**| Year (ex: 2019) |
 **month** | **int**| Month (ex: 01) |

### Return type

[**\Swagger\Client\Model\Article[]**](../Model/Article.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **blogPostPublishedGet**
> \Swagger\Client\Model\Article[] blogPostPublishedGet($featured_only)



Get list of articles published

### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **featured_only** | **bool**|  | [optional]

### Return type

[**\Swagger\Client\Model\Article[]**](../Model/Article.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **blogPostSlugSlugGet**
> \Swagger\Client\Model\Article blogPostSlugSlugGet($slug)



Get list of articles published

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ArticlesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$slug = "slug_example"; // string | Slug of article

try {
    $result = $apiInstance->blogPostSlugSlugGet($slug);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ArticlesApi->blogPostSlugSlugGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **string**| Slug of article |

### Return type

[**\Swagger\Client\Model\Article**](../Model/Article.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

