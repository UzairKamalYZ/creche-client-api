# BabyApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getBaby**](BabyApi.md#getBaby) | **GET** /baby/{id} | create request for baby



## getBaby

> getBaby(id, requestId)

create request for baby

Get Baby details for respective identifier.

### Example

```java
// Import classes:
import com.creche.client.invoker.ApiClient;
import com.creche.client.invoker.ApiException;
import com.creche.client.invoker.Configuration;
import com.creche.client.invoker.models.*;
import com.creche.client.api.BabyApi;

public class Example {
    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        defaultClient.setBasePath("http://localhost");

        BabyApi apiInstance = new BabyApi(defaultClient);
        String id = "id_example"; // String | Baby identifier
        String requestId = "requestId_example"; // String | Help in tracing request
        try {
            apiInstance.getBaby(id, requestId);
        } catch (ApiException e) {
            System.err.println("Exception when calling BabyApi#getBaby");
            System.err.println("Status code: " + e.getCode());
            System.err.println("Reason: " + e.getResponseBody());
            System.err.println("Response headers: " + e.getResponseHeaders());
            e.printStackTrace();
        }
    }
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Baby identifier |
 **requestId** | **String**| Help in tracing request | [optional]

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **400** |  |  -  |

