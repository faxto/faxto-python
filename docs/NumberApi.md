# swagger_client.NumberApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**numbers_get**](NumberApi.md#numbers_get) | **GET** /numbers | 


# **numbers_get**
> numbers_get(api_key, page=page)



This API get users numbers. 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.NumberApi()
api_key = 'api_key_example' # str | API Key
page = 'page_example' # str | Page to display (optional)

try: 
    api_instance.numbers_get(api_key, page=page)
except ApiException as e:
    print("Exception when calling NumberApi->numbers_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **page** | **str**| Page to display | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

