---
title: "[WS] Verify Response Status Code In Range" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/ws-verify-response-status-code-in-range.html 
description: 
---
Description
-----------

Verify status code valid in a range of status codes in the returned data from a web service call.

Parameters
----------

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Parameter</th><th class="" style="">Parameter Type</th><th class="" style="">Mandatory</th><th class="" style="">Description</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style=""><span style="" class="">responseObject</span></td><td class="" style=""><span style="" class="">ResponseObject</span></td><td class="" style="">Required</td><td class="" style=""><span style="" class="">The object represents an HTTP Response, the user can get responded content type, header properties (sometimes the user may want to get cookies from response header)</span></td></tr><tr class="" style=""><td class="" colspan="1" style="">fromStatusCode</td><td class="" colspan="1" style="">int</td><td class="" colspan="1" style="">Required</td><td class="" colspan="1" style="">From status code</td></tr><tr class="" style=""><td class="" colspan="1" style="">toStatusCode</td><td class="" colspan="1" style="">int</td><td class="" colspan="1" style="">Required</td><td class="" colspan="1" style="">To status code</td></tr><tr class="" style=""><td class="" style=""><span style="" class="">flowControl</span></td><td class="" style=""><span style="" class="">FailureHandling</span></td><td class="" style="">Optional</td><td class="" style=""><span style="" class="">Spec</span><span class="" style="">ify </span><a href="https://docs.katalon.com/x/qAAM" rel="nofollow" class="" style="">failure handling</a><span class="" style=""> schema to determine whether the execution should be allowed to continue or stop.</span></td></tr></tbody></table>

Returns
-------

*   **true** if the response status code is the same as the expected status code, otherwise **false**.

Example
-------

You want to verify if the response from "REST\_Status Codes/POST\_201" object returns a status code from 200 to 400.

```
import static com.kms.katalon.core.checkpoint.CheckpointFactory.findCheckpointimport static com.kms.katalon.core.testcase.TestCaseFactory.findTestCase
import static com.kms.katalon.core.testdata.TestDataFactory.findTestData
import static com.kms.katalon.core.testobject.ObjectRepository.findTestObject
import com.kms.katalon.core.checkpoint.Checkpoint as Checkpoint
import com.kms.katalon.core.checkpoint.CheckpointFactory as CheckpointFactory
import com.kms.katalon.core.mobile.keyword.MobileBuiltInKeywords as MobileBuiltInKeywords
import com.kms.katalon.core.mobile.keyword.MobileBuiltInKeywords as Mobile
import com.kms.katalon.core.model.FailureHandling as FailureHandling
import com.kms.katalon.core.testcase.TestCase as TestCase
import com.kms.katalon.core.testcase.TestCaseFactory as TestCaseFactory
import com.kms.katalon.core.testdata.TestData as TestData
import com.kms.katalon.core.testdata.TestDataFactory as TestDataFactory
import com.kms.katalon.core.testobject.ObjectRepository as ObjectRepository
import com.kms.katalon.core.testobject.TestObject as TestObject
import com.kms.katalon.core.webservice.keyword.WSBuiltInKeywords as WSBuiltInKeywords
import com.kms.katalon.core.webservice.keyword.WSBuiltInKeywords as WS
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUiBuiltInKeywords
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUI
import internal.GlobalVariable as GlobalVariable
  
'Send a request and returns its response'
def response = WS.sendRequest(findTestObject('REST_Status Codes/POST_201'))
 
'Verify if the response from "REST_Status Codes/POST_201" object returns a status code from 200 to 400'
WS.verifyResponseStatusCode(response, 201)
```