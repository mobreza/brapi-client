# StudyApi

All URIs are relative to *https://localhost/pippa_experiments*

Method | HTTP request | Description
------------- | ------------- | -------------
[**studyDetails**](StudyApi.md#studyDetails) | **GET** /brapi/v1/studies/{studyDbId} | Returns a list of studies
[**studySearch**](StudyApi.md#studySearch) | **POST** /brapi/v1/studies-search | Returns a list of studies


<a name="studyDetails"></a>
# **studyDetails**
> StudyResult studyDetails(studyDbId)

Returns a list of studies



### Example
```java
// Import classes:
//import org.brapi.client.ApiException;
//import org.brapi.client.api.StudyApi;


StudyApi apiInstance = new StudyApi();
String studyDbId = "studyDbId_example"; // String | Get study by studyDbId
try {
    StudyResult result = apiInstance.studyDetails(studyDbId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StudyApi#studyDetails");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **studyDbId** | **String**| Get study by studyDbId |

### Return type

[**StudyResult**](StudyResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="studySearch"></a>
# **studySearch**
> StudySearchResult studySearch(germplasmDbIds)

Returns a list of studies



### Example
```java
// Import classes:
//import org.brapi.client.ApiException;
//import org.brapi.client.api.StudyApi;


StudyApi apiInstance = new StudyApi();
List<String> germplasmDbIds = Arrays.asList("germplasmDbIds_example"); // List<String> | Filter studies by germplasms used in it
try {
    StudySearchResult result = apiInstance.studySearch(germplasmDbIds);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StudyApi#studySearch");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **germplasmDbIds** | [**List&lt;String&gt;**](String.md)| Filter studies by germplasms used in it | [optional]

### Return type

[**StudySearchResult**](StudySearchResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

