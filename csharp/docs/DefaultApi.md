# IO.Swagger.Api.DefaultApi

All URIs are relative to *https://virtserver.swaggerhub.com/cwelt/CustomerAPI/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetCustomer**](DefaultApi.md#getcustomer) | **GET** /customer | reads a customer&#39;s data


<a name="getcustomer"></a>
# **GetCustomer**
> InlineResponse200 GetCustomer (int? customerId)

reads a customer's data

This operation provides a view of customer's view in JSON. The operation uses the customer's Id to identify the customer in the query string.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetCustomerExample
    {
        public void main()
        {
            var apiInstance = new DefaultApi();
            var customerId = 56;  // int? | pass an optional customer id.

            try
            {
                // reads a customer's data
                InlineResponse200 result = apiInstance.GetCustomer(customerId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling DefaultApi.GetCustomer: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerId** | **int?**| pass an optional customer id. | 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

