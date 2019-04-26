# Swagger\Client\DefaultApi

All URIs are relative to *http://hytale.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**blogPostArchiveYearMonthGet**](DefaultApi.md#blogPostArchiveYearMonthGet) | **GET** /blog/post/archive/{year}/{month}/ | 
[**blogPostPublishedGet**](DefaultApi.md#blogPostPublishedGet) | **GET** /blog/post/published | 
[**blogPostSlugSlugGet**](DefaultApi.md#blogPostSlugSlugGet) | **GET** /blog/post/slug/{slug} | 
[**jobListingGet**](DefaultApi.md#jobListingGet) | **GET** /job/listing | 


# **blogPostArchiveYearMonthGet**
> blogPostArchiveYearMonthGet($year, $month)



Get list of articles published on a specific month of an year

### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **int**| Year (ex: 2019) |
 **month** | **int**| Month (ex: 01) |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **blogPostPublishedGet**
> blogPostPublishedGet($featured_only)



Get list of articles published

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$featured_only = true; // bool | 

try {
    $apiInstance->blogPostPublishedGet($featured_only);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->blogPostPublishedGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **featured_only** | **bool**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **blogPostSlugSlugGet**
> blogPostSlugSlugGet($slug)



Get list of articles published

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$slug = "slug_example"; // string | Slug of article

try {
    $apiInstance->blogPostSlugSlugGet($slug);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->blogPostSlugSlugGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **string**| Slug of article |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **jobListingGet**
> jobListingGet()



Get list of jobs

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->jobListingGet();
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->jobListingGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

