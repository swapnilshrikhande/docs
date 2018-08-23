---
title: "[WebUI] Get Window Title" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/webui-get-window-title.html 
description: 
---
Description  
-------------

Get the title of the current window.

Parameters  
------------

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Param</th><th class="" style="">Param Type</th><th class="" colspan="1" style="">Mandatory</th><th class="" colspan="1" style="">Description</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style=""><span style="" class="">flowControl</span></td><td class="" style=""><span style="" class="">FailureHandling</span></td><td class="" colspan="1" style=""><span style="" class="">Optional</span></td><td class="" colspan="1" style="">Specify <a href="https://docs.katalon.com/x/qAAM" rel="nofollow" class="" style="">failure handling</a> <span style="" class="">schema to determine whether the execution should be allowed to continue or stop.</span></td></tr></tbody></table>

Returns
-------

<table class="" style="table-layout: fixed;"><thead class="" style=""><tr class="" style=""><th class="" style=""><div class="" style="">Param Type</div></th><th class="" style=""><div class="" style="">Description</div></th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style=""><span style="" class="">String</span></td><td class="" style=""><p class="" style=""><span style="" class="">Title&nbsp;of the current window.</span></p></td></tr></tbody></table>

Example 
--------

You want to get the title of the current window. The output is stored in variable "title".

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

'Open browser and navigate to website katalon.com'
WebUI.openBrowser('https://www.katalon.com/')

'Click on Documentation to open another window'
WebUI.click(findTestObject('Page_Katalon Studio/a_Documentation'))

'Switch to Documentation window'
WebUI.switchToWindowIndex(1)

'Get title of Documentation window'
title = WebUI.getWindowTitle()

'Close browser'
WebUI.closeBrowser()
```