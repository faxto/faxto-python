# swagger_client.CountryApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**areacodes_country_code_state_id_get**](CountryApi.md#areacodes_country_code_state_id_get) | **GET** /areacodes/{countryCode}/{stateId} | 
[**countries_country_code_didgroups_get**](CountryApi.md#countries_country_code_didgroups_get) | **GET** /countries/{countryCode}/didgroups | 
[**countries_didgroups_did_group_id_provision_post**](CountryApi.md#countries_didgroups_did_group_id_provision_post) | **POST** /countries/didgroups/{didGroupId}/provision | 
[**countries_get**](CountryApi.md#countries_get) | **GET** /countries | 
[**states_country_code_get**](CountryApi.md#states_country_code_get) | **GET** /states/{countryCode} | 


# **areacodes_country_code_state_id_get**
> areacodes_country_code_state_id_get(country_code, state_id)



This API get areacodes . 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.CountryApi()
country_code = 'country_code_example' # str | countryCode in the Country
state_id = 'state_id_example' # str | stateId in the Country

try: 
    api_instance.areacodes_country_code_state_id_get(country_code, state_id)
except ApiException as e:
    print("Exception when calling CountryApi->areacodes_country_code_state_id_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country_code** | **str**| countryCode in the Country | 
 **state_id** | **str**| stateId in the Country | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **countries_country_code_didgroups_get**
> countries_country_code_didgroups_get(country_code, did_group_ids, state_id, city_name_pattern)



This API didgroups countryCode. 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.CountryApi()
country_code = 'country_code_example' # str | countryCode in the Country
did_group_ids = 'did_group_ids_example' # str | didGroupId in the Country
state_id = 'state_id_example' # str | stateId in the Country
city_name_pattern = 'city_name_pattern_example' # str | cityNamePattern in the Country

try: 
    api_instance.countries_country_code_didgroups_get(country_code, did_group_ids, state_id, city_name_pattern)
except ApiException as e:
    print("Exception when calling CountryApi->countries_country_code_didgroups_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country_code** | **str**| countryCode in the Country | 
 **did_group_ids** | **str**| didGroupId in the Country | 
 **state_id** | **str**| stateId in the Country | 
 **city_name_pattern** | **str**| cityNamePattern in the Country | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **countries_didgroups_did_group_id_provision_post**
> countries_didgroups_did_group_id_provision_post(did_group_id)



This API didgroups provision. 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.CountryApi()
did_group_id = 'did_group_id_example' # str | didGroupId in the Country

try: 
    api_instance.countries_didgroups_did_group_id_provision_post(did_group_id)
except ApiException as e:
    print("Exception when calling CountryApi->countries_didgroups_did_group_id_provision_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **did_group_id** | **str**| didGroupId in the Country | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **countries_get**
> countries_get()



This API get countries. 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.CountryApi()

try: 
    api_instance.countries_get()
except ApiException as e:
    print("Exception when calling CountryApi->countries_get: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **states_country_code_get**
> states_country_code_get(country_code)



This API get States . 

### Example 
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.CountryApi()
country_code = 'country_code_example' # str | countryCode in the Country

try: 
    api_instance.states_country_code_get(country_code)
except ApiException as e:
    print("Exception when calling CountryApi->states_country_code_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country_code** | **str**| countryCode in the Country | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

