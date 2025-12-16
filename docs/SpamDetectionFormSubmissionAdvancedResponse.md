# SpamDetectionFormSubmissionAdvancedResponse

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CleanResult** | **bool** | True if the result is not spam (clean), and false otherwise | [optional] [default to null]
**SpamRiskLevel** | **float64** | Overall spam risk level between 0.0 and 1.0 | [optional] [default to null]
**ContainsSpam** | **bool** | True if the input text contains spam, false otherwise | [optional] [default to null]
**ContainsUnsolicitedSales** | **bool** | True if the input text contains unsolicited sales, false otherwise | [optional] [default to null]
**ContainsPromotionalContent** | **bool** | True if the input text contains promotional content, false otherwise | [optional] [default to null]
**ContainsPhishingAttempt** | **bool** | True if the input text contains a phishing attempt, false otherwise | [optional] [default to null]
**AnalysisRationale** | **string** | Rationale for why the conclusion was formed | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


