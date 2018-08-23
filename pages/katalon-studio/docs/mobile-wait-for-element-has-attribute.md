---
title: "[Mobile] Wait For Element Has Attribute" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/mobile-wait-for-element-has-attribute.html 
description: 
---
Description
-----------

Wait until the given mobile element has an attribute with the specified name.

Parameters
----------

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Param</th><th class="" colspan="1" style="">Param Type</th><th class="" colspan="1" style="">Mandatory</th><th class="" style="">Description</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style=""><span style="" class="">to</span></td><td class="" colspan="1" style="">TestObject</td><td class="" colspan="1" style="">Required</td><td class="" style=""><p class="" style=""><span style="" class="">Represent a mobile element.</span></p></td></tr><tr class="" style=""><td class="" colspan="1" style=""><span style="" class="">attributeName</span></td><td class="" colspan="1" style="">String</td><td class="" colspan="1" style="">Required</td><td class="" colspan="1" style=""><span style="" class="">The name of the attribute to wait for.</span></td></tr><tr class="" style=""><td class="" colspan="1" style="">timeout</td><td class="" colspan="1" style="">int</td><td class="" colspan="1" style="">Required</td><td class="" colspan="1" style=""><span style="" class="">System will wait at most timeout (seconds) to return a result</span></td></tr><tr class="" style=""><td class="" style=""><span style="" class="">flowControl</span></td><td class="" colspan="1" style="">FailureHandling</td><td class="" colspan="1" style="">Optional</td><td class="" style=""><span style="" class="">Spec</span><span class="" style="">ify </span><a href="https://docs.katalon.com/x/qAAM" rel="nofollow" class="" style="">failure handling</a><span class="" style=""> schema to determine whether the execution should be allowed to continue or stop.</span></td></tr></tbody></table>

Returns
-------

<table class="" style="table-layout: fixed;"><thead><tr><th class="" colspan="1" style="">Param Type</th><th class="" style="">Description</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" colspan="1" style="">boolean</td><td class="" style=""><ul class="" style=""><li class="" style=""><strong class="" style="">true:</strong> the element has the attribute with the specified name.</li><li class="" style=""><strong class="" style="">false: </strong>the element doesn't have the attribute with the specified name.</li></ul></td></tr></tbody></table>

Example
-------

You want to wait for 'App' button has 'class' attribute.

```
import static com.kms.katalon.core.testcase.TestCaseFactory.findTestCase
import static com.kms.katalon.core.testdata.TestDataFactory.findTestData
import static com.kms.katalon.core.testobject.ObjectRepository.findTestObject
import internal.GlobalVariable as GlobalVariable
import com.kms.katalon.core.configuration.RunConfiguration as RunConfiguration
import com.kms.katalon.core.mobile.keyword.MobileBuiltInKeywords as Mobile
import com.kms.katalon.core.util.internal.PathUtil as PathUtil
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUI
import com.kms.katalon.core.webservice.keyword.WSBuiltInKeywords as WS
import static com.kms.katalon.core.checkpoint.CheckpointFactory.findCheckpoint
import com.kms.katalon.core.model.FailureHandling as FailureHandling
import com.kms.katalon.core.testcase.TestCase as TestCase
import com.kms.katalon.core.testdata.TestData as TestData
import com.kms.katalon.core.testobject.TestObject as TestObject
import com.kms.katalon.core.checkpoint.Checkpoint as Checkpoint

'Start application on current selected android\'s device'
Mobile.startApplication(GlobalVariable.G_AndroidApp, false)

'Wait until app control has class atribute'
Mobile.waitForElementHasAttribute(findTestObject(findTestObject('Object Repository/Application/android.widget.TextView - App')), 'class', 20)

'Close application on current selected android\'s device'
Mobile.closeApplication()
```

###### Wait until the given web element has an attribute with the specific name

###### Parameters:  

*   to - TestObject (required): represent a mobile element
    
*   attributeName - String (required): the name of the attribute to verify
    
*   timeOut - int (required): \- system will wait at most timeout (seconds) to return result
    
*   flowControl - FailureHandling (optional): specify failure handling schema to determine whether the execution should be allowed to continue or stop. More details is in this page: [Failure Handling](/display/KD/Failure+Handling)

#### Returns

**true** if element has the attribute with the specific name; otherwise, **false**

#### Example: You want to wait until the button has an attribute with name = 'class'

Manual: 

** ![](../../images/katalon-studio/docs/mobile-wait-for-element-has-attribute/image2016-8-15 19_2_59.png)**

Script:

```
Mobile.waitForElementHasAttribute(findTestObject('SampleApp.apk/android.widget.Button - Button0'), 'class', 10)
```