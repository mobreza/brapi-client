# GermplasmApi

All URIs are relative to *https://localhost/pippa_experiments*

Method | HTTP request | Description
------------- | ------------- | -------------
[**germplasmSearch**](GermplasmApi.md#germplasmSearch) | **GET** /brapi/v1/germplasm-search | Returns a list of germplasms


<a name="germplasmSearch"></a>
# **germplasmSearch**
> GermplasmSearchResult germplasmSearch(germplasmDbId, germplasmSpecies, germplasmName, pageSize, page)

Returns a list of germplasms



### Example
```java
// Import classes:
//import org.brapi.client.ApiException;
//import org.brapi.client.api.GermplasmApi;


GermplasmApi apiInstance = new GermplasmApi();
Integer germplasmDbId = 56; // Integer | Filter germplasms by database id
String germplasmSpecies = "germplasmSpecies_example"; // String | Filter germplasms by species name
String germplasmName = "germplasmName_example"; // String | Filter measurements by variable id
Integer pageSize = 56; // Integer | Size of page
Integer page = 56; // Integer | Page number
try {
    GermplasmSearchResult result = apiInstance.germplasmSearch(germplasmDbId, germplasmSpecies, germplasmName, pageSize, page);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GermplasmApi#germplasmSearch");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **germplasmDbId** | **Integer**| Filter germplasms by database id | [optional]
 **germplasmSpecies** | **String**| Filter germplasms by species name | [optional]
 **germplasmName** | **String**| Filter measurements by variable id | [optional]
 **pageSize** | **Integer**| Size of page | [optional]
 **page** | **Integer**| Page number | [optional]

### Return type

[**GermplasmSearchResult**](GermplasmSearchResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

