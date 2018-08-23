---
title: "[WebUI] Verify Element Visible In Viewport" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/webui-verify-element-visible-in-viewport.html 
description: 
---
Description
-----------

Verify if the web element is visible in current [viewport](https://www.w3schools.com/css/css_rwd_viewport.asp)

Parameters
----------

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Param</th><th class="" style="">Param Type</th><th class="" colspan="1" style="">Mandatory</th><th class="" colspan="1" style="">Description</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" colspan="1" style=""><span style="" class="">to</span></td><td class="" colspan="1" style=""><span style="" class="">TestObject</span></td><td class="" colspan="1" style=""><span style="" class="">Required</span></td><td class="" colspan="1" style=""><span style="" class="">Represent a web element.</span></td></tr><tr class="" style=""><td class="" colspan="1" style=""><span style="" class="">timeOut&nbsp;</span></td><td class="" colspan="1" style=""><span style="" class="">int&nbsp;</span></td><td class="" colspan="1" style=""><span style="" class="">Required</span></td><td class="" colspan="1" style=""><span style="" class="">Maximum period of time (in seconds) that system will wait to return the result.</span></td></tr><tr class="" style=""><td class="" style=""><span style="" class="">flowControl</span></td><td class="" style=""><span style="" class="">FailureHandling</span></td><td class="" colspan="1" style=""><span style="" class="">Optional</span></td><td class="" colspan="1" style=""><span style="" class="">Specify <span style="" class=""><a href="https://docs.katalon.com/x/qAAM" rel="nofollow" class="" style="">failure handling</a></span> schema to determine whether the execution should be allowed to continue or stop.</span></td></tr></tbody></table>

Returns
-------

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Param Type</th><th class="" style="">Description</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style=""><span style="" class="">Boolean</span></td><td class="" style=""><ul class="" style=""><li class="" style=""><span style="" class=""><strong class="" style="">true:</strong>&nbsp;the element is visible in current viewport.</span></li><li class="" style=""><span style="" class=""><strong class="" style="">false:</strong> the element is NOT visible in current viewport.</span></li></ul></td></tr></tbody></table>

Example
-------

You want to verify 'btn_Login' button to be visible in 10 seconds in the current viewport.

```
import static com.kms.katalon.core.checkpoint.CheckpointFactory.findCheckpoint
import static com.kms.katalon.core.testcase.TestCaseFactory.findTestCase
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

'Open browser and navigate to website that contains the element to wait for'
WebUI.openBrowser(GlobalVariable.G_SiteURL)

'Wait for btn_Login to be visible in 10s'
WebUI.verifyElementVisibleInViewport(findTestObject('Page_Login/btn_Login'), 10)

'Close browser'
WebUI.closeBrowser()
```