# PhenotypeApi

All URIs are relative to *https://localhost/pippa_experiments*

Method | HTTP request | Description
------------- | ------------- | -------------
[**phenotypeSearch**](PhenotypeApi.md#phenotypeSearch) | **POST** /brapi/v1/phenotype-search | Returns a list of phenotypes


<a name="phenotypeSearch"></a>
# **phenotypeSearch**
> PhenotypeSearchResult phenotypeSearch(germplasmDbIds, studyDbIds, programDbIds, observationVariableDbIds, pageSize, page)

Returns a list of phenotypes

Note: the API definition here is subject to change...

### Example
```java
// Import classes:
//import org.brapi.client.ApiException;
//import org.brapi.client.api.PhenotypeApi;


PhenotypeApi apiInstance = new PhenotypeApi();
String germplasmDbIds = "germplasmDbIds_example"; // String | Filter phenotypes by germplasm database ids
String studyDbIds = "studyDbIds_example"; // String | Filter phenotypes by study database ids
String programDbIds = "programDbIds_example"; // String | Filter phenotypes by program database ids
String observationVariableDbIds = "observationVariableDbIds_example"; // String | Filter phenotypes by observation variable database ids
Integer pageSize = 56; // Integer | Size of page
Integer page = 56; // Integer | Page number
try {
    PhenotypeSearchResult result = apiInstance.phenotypeSearch(germplasmDbIds, studyDbIds, programDbIds, observationVariableDbIds, pageSize, page);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PhenotypeApi#phenotypeSearch");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **germplasmDbIds** | **String**| Filter phenotypes by germplasm database ids | [optional]
 **studyDbIds** | **String**| Filter phenotypes by study database ids | [optional]
 **programDbIds** | **String**| Filter phenotypes by program database ids | [optional]
 **observationVariableDbIds** | **String**| Filter phenotypes by observation variable database ids | [optional]
 **pageSize** | **Integer**| Size of page | [optional]
 **page** | **Integer**| Page number | [optional]

### Return type

[**PhenotypeSearchResult**](PhenotypeSearchResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

