# swagger_client.FaxApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fax_document_id_costs_get**](FaxApi.md#fax_document_id_costs_get) | **GET** /fax/{document_id}/costs | 
[**fax_get**](FaxApi.md#fax_get) | **GET** /fax | 
[**fax_job_id_status_get**](FaxApi.md#fax_job_id_status_get) | **GET** /fax/{job_id}/status | 
[**incoming_faxes_get**](FaxApi.md#incoming_faxes_get) | **GET** /incoming-faxes | 
[**incoming_faxes_number_get**](FaxApi.md#incoming_faxes_number_get) | **GET** /incoming-faxes/{number} | 
[**provision_numbers_get**](FaxApi.md#provision_numbers_get) | **GET** /provision-numbers | 


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

# **fax_get**
> fax_get(api_key, limit=limit, page=page)



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
    api_instance.fax_get(api_key, limit=limit, page=page)
except ApiException as e:
    print("Exception when calling FaxApi->fax_get: %s\n" % e)
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

# **incoming_faxes_get**
> incoming_faxes_get(api_key)



This API get faxes . 

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

try: 
    api_instance.incoming_faxes_get(api_key)
except ApiException as e:
    print("Exception when calling FaxApi->incoming_faxes_get: %s\n" % e)
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

# **incoming_faxes_number_get**
> incoming_faxes_number_get(api_key, number)



This API get faxes  by number. 

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
number = 'number_example' # str | Number in the fax

try: 
    api_instance.incoming_faxes_number_get(api_key, number)
except ApiException as e:
    print("Exception when calling FaxApi->incoming_faxes_number_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **number** | **str**| Number in the fax | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **provision_numbers_get**
> provision_numbers_get(api_key, limit=limit)



This API get Provision numbers. 

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
limit = 'limit_example' # str | Limit to display (optional)

try: 
    api_instance.provision_numbers_get(api_key, limit=limit)
except ApiException as e:
    print("Exception when calling FaxApi->provision_numbers_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **str**| API Key | 
 **limit** | **str**| Limit to display | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

