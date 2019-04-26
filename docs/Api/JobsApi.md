# Swagger\Client\JobsApi

All URIs are relative to *http://hytale.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getJobs**](JobsApi.md#getJobs) | **GET** /job/listing | 


# **getJobs**
> \Swagger\Client\Model\Job[] getJobs()



Get list of jobs

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\JobsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->getJobs();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling JobsApi->getJobs: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\Job[]**](../Model/Job.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

