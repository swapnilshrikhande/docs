---
title: "[WebUI] Verify Image Present" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/webui-verify-image-present.html 
description: 
---
Description 
------------

Verify if an image is present on page.

Parameters 
-----------

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Param</th><th class="" style="">Param Type</th><th class="" colspan="1" style="">Mandatory</th><th class="" colspan="1" style="">Description</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" colspan="1" style="">to</td><td class="" colspan="1" style="">TestObject</td><td class="" colspan="1" style="">Required</td><td class="" colspan="1" style="">Represent an image.</td></tr><tr class="" style=""><td class="" style=""><span style="" class="">flowControl</span></td><td class="" style=""><span style="" class="">FailureHandling</span></td><td class="" colspan="1" style="">Optional</td><td class="" colspan="1" style=""><span style="" class="">Spec</span><span class="" style="">ify </span><a href="https://docs.katalon.com/x/qAAM" rel="nofollow" class="" style="">failure handling</a><span class="" style=""> schema to determine whether the execution should be allowed to continue or stop.</span></td></tr></tbody></table>

Returns 
--------

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Param Type</th><th class="" style="">Description</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style=""><span style="" class="">Boolean</span></td><td class="" style=""><ul class="" style=""><li class="" style=""><p class="" style=""><span style="" class="">true&nbsp;if the image if present.</span></p></li><li class="" style=""><p class="" style=""><span style="" class="">false&nbsp;if the image is not present.</span><span style="" class="">&nbsp;</span></p></li></ul></td></tr></tbody></table>

Example 
--------

You want to verify if "img_KatalonLogo" is present on page.

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

'Open browser and navigate to a site that contains an image'
WebUI.openBrowser(GlobalVariable.G_SiteURL)

'Verify if the image is present'
WebUI.verifyImagePresent(findTestObject('img_KatalonLogo'))

'Close browser'
WebUI.closeBrowser()


```

The test object needs to define a source image from the local machine for Katalon Studio to use it for verification

![](../../images/katalon-studio/docs/webui-verify-image-present/define_image.jpg)