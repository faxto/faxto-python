# swagger_client.FilesApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**file_clean_get**](FilesApi.md#file_clean_get) | **GET** /file-clean | 
[**file_generate_preview_get**](FilesApi.md#file_generate_preview_get) | **GET** /file-generate-preview | 
[**files_get**](FilesApi.md#files_get) | **GET** /files | 
[**files_id_delete**](FilesApi.md#files_id_delete) | **DELETE** /files/{id} | 
[**files_post**](FilesApi.md#files_post) | **POST** /files | 


# **file_clean_get**
> file_clean_get(api_key, document_id)



This API get clean file from document id. 

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
document_id = 'document_id_example' # str | Document ID in the fax

try: 
    api_instance.file_clean_get(api_key, document_id)
except ApiException as e:
    print("Exception when calling FilesApi->file_clean_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **document_id** | **str**| Document ID in the fax | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **file_generate_preview_get**
> file_generate_preview_get(api_key, document_id)



This API get generated preview file from document id. 

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
document_id = 'document_id_example' # str | Document ID in the fax

try: 
    api_instance.file_generate_preview_get(api_key, document_id)
except ApiException as e:
    print("Exception when calling FilesApi->file_generate_preview_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **document_id** | **str**| Document ID in the fax | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

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
> File files_post(api_key, file, add_remote_file=add_remote_file)



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
add_remote_file = 'add_remote_file_example' # str | Given the remote file url (optional)

try: 
    api_response = api_instance.files_post(api_key, file, add_remote_file=add_remote_file)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling FilesApi->files_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **file** | **file**| PDF file to upload | 
 **add_remote_file** | **str**| Given the remote file url | [optional] 

### Return type

[**File**](File.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

