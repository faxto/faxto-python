# swagger_client.FaxApi

All URIs are relative to *https://fax.to/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fax_document_id_costs_get**](FaxApi.md#fax_document_id_costs_get) | **GET** /fax/{document_id}/costs | 
[**fax_history_get**](FaxApi.md#fax_history_get) | **GET** /fax-history | 
[**fax_job_id_status_get**](FaxApi.md#fax_job_id_status_get) | **GET** /fax/{job_id}/status | 
[**fax_post**](FaxApi.md#fax_post) | **POST** /fax | 


# **fax_document_id_costs_get**
> fax_document_id_costs_get(api_key, fax_number, document_id)



This API get the cost of a sending fax. 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.FaxApi()
api_key = 'api_key_example' # str | API Key
fax_number = 'fax_number_example' # str | Fax Number
document_id = 3.4 # float | id of the file / document_id

try: 
    api_instance.fax_document_id_costs_get(api_key, fax_number, document_id)
except ApiException as e:
    print("Exception when calling FaxApi->fax_document_id_costs_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **fax_number** | **str**| Fax Number | 
 **document_id** | **float**| id of the file / document_id | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fax_history_get**
> fax_history_get(api_key, limit=limit, page=page)



This API get all fax history. 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.FaxApi()
api_key = 'api_key_example' # str | API Key
limit = 'limit_example' # str | Number of records to return (optional)
page = 'page_example' # str | Page to display (optional)

try: 
    api_instance.fax_history_get(api_key, limit=limit, page=page)
except ApiException as e:
    print("Exception when calling FaxApi->fax_history_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **limit** | **str**| Number of records to return | [optional] 
 **page** | **str**| Page to display | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fax_job_id_status_get**
> fax_job_id_status_get(api_key, job_id)



This API get the status of the fax. 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.FaxApi()
api_key = 'api_key_example' # str | API Key
job_id = 3.4 # float | id of the fax job

try: 
    api_instance.fax_job_id_status_get(api_key, job_id)
except ApiException as e:
    print("Exception when calling FaxApi->fax_job_id_status_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **job_id** | **float**| id of the fax job | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fax_post**
> fax_post(api_key, fax_number, document_id=document_id, tsi_number=tsi_number, file=file, delete_file=delete_file)



This API send the fax. When we send fax using API, Fax.to send a POST to the Callback URL you specified in https://fax.to/member/api/live. Fax.to send POST data with the following information fax_job_id, status and message. 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.FaxApi()
api_key = 'api_key_example' # str | API Key
fax_number = 'fax_number_example' # str | Fax Number
document_id = 56 # int | Document id. If you want to use existing document you need to specify the document_id (optional)
tsi_number = 'tsi_number_example' # str | If we want to to change the text or number that appear on 'from' or 'sender' of the fax (optional)
file = '/path/to/file.txt' # file | PDF file to upload (optional)
delete_file = 56 # int | Whether to delete file after fax transaction. (put 1 to delete) (optional)

try: 
    api_instance.fax_post(api_key, fax_number, document_id=document_id, tsi_number=tsi_number, file=file, delete_file=delete_file)
except ApiException as e:
    print("Exception when calling FaxApi->fax_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **fax_number** | **str**| Fax Number | 
 **document_id** | **int**| Document id. If you want to use existing document you need to specify the document_id | [optional] 
 **tsi_number** | **str**| If we want to to change the text or number that appear on &#39;from&#39; or &#39;sender&#39; of the fax | [optional] 
 **file** | **file**| PDF file to upload | [optional] 
 **delete_file** | **int**| Whether to delete file after fax transaction. (put 1 to delete) | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

