# swagger-client
No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)

This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 0.0.1
- Package version: 1.0.0
- Build package: io.swagger.codegen.languages.PythonClientCodegen

## Requirements.

Python 2.7 and 3.4+

## Installation & Usage
### pip install

If the python package is hosted on Github, you can install directly from Github

```sh
pip install git+https://github.com//.git
```
(you may need to run `pip` with root permission: `sudo pip install git+https://github.com//.git`)

Then import the package:
```python
import swagger_client 
```

### Setuptools

Install via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install --user
```
(or `sudo python setup.py install` to install the package for all users)

Then import the package:
```python
import swagger_client
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint
# create an instance of the API class
api_instance = swagger_client.AccountApi()
api_key = 'api_key_example' # str | API Key

try:
    api_instance.balance_get(api_key)
except ApiException as e:
    print("Exception when calling AccountApi->balance_get: %s\n" % e)

```

## Documentation for API Endpoints

All URIs are relative to *https://fax.to/api/v2*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AccountApi* | [**balance_get**](docs/AccountApi.md#balance_get) | **GET** /balance | 
*CountryApi* | [**areacodes_country_code_state_id_get**](docs/CountryApi.md#areacodes_country_code_state_id_get) | **GET** /areacodes/{countryCode}/{stateId} | 
*CountryApi* | [**countries_country_code_didgroups_get**](docs/CountryApi.md#countries_country_code_didgroups_get) | **GET** /countries/{countryCode}/didgroups | 
*CountryApi* | [**countries_didgroups_did_group_id_provision_post**](docs/CountryApi.md#countries_didgroups_did_group_id_provision_post) | **POST** /countries/didgroups/{didGroupId}/provision | 
*CountryApi* | [**countries_get**](docs/CountryApi.md#countries_get) | **GET** /countries | 
*CountryApi* | [**states_country_code_get**](docs/CountryApi.md#states_country_code_get) | **GET** /states/{countryCode} | 
*FaxApi* | [**fax_document_id_costs_get**](docs/FaxApi.md#fax_document_id_costs_get) | **GET** /fax/{document_id}/costs | 
*FaxApi* | [**fax_get**](docs/FaxApi.md#fax_get) | **GET** /fax | 
*FaxApi* | [**fax_job_id_status_get**](docs/FaxApi.md#fax_job_id_status_get) | **GET** /fax/{job_id}/status | 
*FaxApi* | [**incoming_faxes_get**](docs/FaxApi.md#incoming_faxes_get) | **GET** /incoming-faxes | 
*FaxApi* | [**incoming_faxes_number_get**](docs/FaxApi.md#incoming_faxes_number_get) | **GET** /incoming-faxes/{number} | 
*FaxApi* | [**provision_numbers_get**](docs/FaxApi.md#provision_numbers_get) | **GET** /provision-numbers | 
*FilesApi* | [**file_clean_get**](docs/FilesApi.md#file_clean_get) | **GET** /file-clean | 
*FilesApi* | [**file_generate_preview_get**](docs/FilesApi.md#file_generate_preview_get) | **GET** /file-generate-preview | 
*FilesApi* | [**files_get**](docs/FilesApi.md#files_get) | **GET** /files | 
*FilesApi* | [**files_id_delete**](docs/FilesApi.md#files_id_delete) | **DELETE** /files/{id} | 
*FilesApi* | [**files_post**](docs/FilesApi.md#files_post) | **POST** /files | 
*NumberApi* | [**numbers_get**](docs/NumberApi.md#numbers_get) | **GET** /numbers | 


## Documentation For Models

 - [File](docs/File.md)


## Documentation For Authorization

 All endpoints do not require authorization.


## Author



