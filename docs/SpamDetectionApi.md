# \SpamDetectionApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SpamDetectFileAdvancedPost**](SpamDetectionApi.md#SpamDetectFileAdvancedPost) | **Post** /spam/detect/file/advanced | Perform advanced AI spam detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.
[**SpamDetectFilePost**](SpamDetectionApi.md#SpamDetectFilePost) | **Post** /spam/detect/file | Perform AI spam detection and classification on an input image or document (PDF or DOCX).  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 100-125 API calls depending on model selected.
[**SpamDetectFormSubmissionAdvancedPost**](SpamDetectionApi.md#SpamDetectFormSubmissionAdvancedPost) | **Post** /spam/detect/form-submission/advanced | Perform advanced AI spam detection and classification against a form submission.  Analyzes form input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.
[**SpamDetectTextStringAdvancedPost**](SpamDetectionApi.md#SpamDetectTextStringAdvancedPost) | **Post** /spam/detect/text-string/advanced | Perform advanced AI spam detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.
[**SpamDetectTextStringPost**](SpamDetectionApi.md#SpamDetectTextStringPost) | **Post** /spam/detect/text-string | Perform AI spam detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-75 API calls depending on model selected.


# **SpamDetectFileAdvancedPost**
> SpamDetectionAdvancedResponse SpamDetectFileAdvancedPost(ctx, optional)
Perform advanced AI spam detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SpamDetectionApiSpamDetectFileAdvancedPostOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SpamDetectionApiSpamDetectFileAdvancedPostOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model** | **optional.String**| Optional: Specify which AI model to use.  Possible choices are Normal and Advanced.  Default is Advanced. | [default to Advanced]
 **preprocessing** | **optional.String**| Optional: Specify which preprocessing to Use.  Possible choices are None, Compatability and Auto.  Default is Auto. | [default to Auto]
 **allowPhishing** | **optional.Bool**| True if phishing should be allowed, false otherwise | [default to false]
 **allowUnsolicitedSales** | **optional.Bool**| True if unsolicited sales should be allowed, false otherwise | [default to false]
 **allowPromotionalContent** | **optional.Bool**| True if promotional content should be allowed, false otherwise | [default to true]
 **inputFile** | **optional.Interface of *os.File**|  | 

### Return type

[**SpamDetectionAdvancedResponse**](SpamDetectionAdvancedResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SpamDetectFilePost**
> SpamDetectionResponse SpamDetectFilePost(ctx, optional)
Perform AI spam detection and classification on an input image or document (PDF or DOCX).  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 100-125 API calls depending on model selected.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SpamDetectionApiSpamDetectFilePostOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SpamDetectionApiSpamDetectFilePostOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model** | **optional.String**| Model to use; default setting is Advanced | [default to Advanced]
 **inputFile** | **optional.Interface of *os.File**|  | 

### Return type

[**SpamDetectionResponse**](SpamDetectionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SpamDetectFormSubmissionAdvancedPost**
> SpamDetectionFormSubmissionAdvancedResponse SpamDetectFormSubmissionAdvancedPost(ctx, optional)
Perform advanced AI spam detection and classification against a form submission.  Analyzes form input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SpamDetectionApiSpamDetectFormSubmissionAdvancedPostOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SpamDetectionApiSpamDetectFormSubmissionAdvancedPostOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of SpamDetectionAdvancedFormSubmissionRequest**](SpamDetectionAdvancedFormSubmissionRequest.md)| Spam detection request | 

### Return type

[**SpamDetectionFormSubmissionAdvancedResponse**](SpamDetectionFormSubmissionAdvancedResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SpamDetectTextStringAdvancedPost**
> SpamDetectionAdvancedResponse SpamDetectTextStringAdvancedPost(ctx, optional)
Perform advanced AI spam detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-100 API calls depending on model selected.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SpamDetectionApiSpamDetectTextStringAdvancedPostOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SpamDetectionApiSpamDetectTextStringAdvancedPostOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of SpamDetectionAdvancedRequest**](SpamDetectionAdvancedRequest.md)| Spam detection request | 

### Return type

[**SpamDetectionAdvancedResponse**](SpamDetectionAdvancedResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **SpamDetectTextStringPost**
> SpamDetectionResponse SpamDetectTextStringPost(ctx, optional)
Perform AI spam detection and classification against input text string.  Analyzes input content as well as embedded URLs with AI deep learnign to detect spam, phishing and other unsafe content.  Uses 25-75 API calls depending on model selected.

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SpamDetectionApiSpamDetectTextStringPostOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SpamDetectionApiSpamDetectTextStringPostOpts struct

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of SpamDetectionRequest**](SpamDetectionRequest.md)| Spam detection request | 

### Return type

[**SpamDetectionResponse**](SpamDetectionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

