# swagger_client.FilesApi

All URIs are relative to *https://fax.to/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**files_get**](FilesApi.md#files_get) | **GET** /files | 
[**files_id_delete**](FilesApi.md#files_id_delete) | **DELETE** /files/{id} | 
[**files_post**](FilesApi.md#files_post) | **POST** /files | 


# **files_get**
> files_get(api_key)



This API lists all the files 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.FilesApi()
api_key = 'api_key_example' # str | API Key

try: 
    api_instance.files_get(api_key)
except ApiException as e:
    print("Exception when calling FilesApi->files_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **files_id_delete**
> files_id_delete(api_key, id)



This API deletes a single file. 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.FilesApi()
api_key = 'api_key_example' # str | API Key
id = 3.4 # float | id of the file / document

try: 
    api_instance.files_id_delete(api_key, id)
except ApiException as e:
    print("Exception when calling FilesApi->files_id_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **id** | **float**| id of the file / document | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **files_post**
> File files_post(api_key, file)



This API allows uploading of a single file. 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.FilesApi()
api_key = 'api_key_example' # str | API Key
file = '/path/to/file.txt' # file | PDF file to upload

try: 
    api_response = api_instance.files_post(api_key, file)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling FilesApi->files_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **file** | **file**| PDF file to upload | 

### Return type

[**File**](File.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

