---
title: "SOAP (latest)" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/soap-latest.html 
description: 
---
1.  Select **File > New > Web Service Request** from the main menu. The **New Web Service Request** dialog will be displayed. Select 'SOAP' from Request Type list to create a new SOAP object.  
    ![](../../images/katalon-studio/docs/soap-latest/Screen Shot 2018-04-05 at 10.55.33 AM.png)  
      
    
2.  A new service request object is created under **Object Repository** of Katalon Studio.  
    ![](../../images/katalon-studio/docs/soap-latest/Screen Shot 2018-04-05 at 10.54.07 AM.png)  
      
    
3.  In the opened editor of the new service request object, enter all required information.  
    ![](../../images/katalon-studio/docs/soap-latest/Screen Shot 2018-04-05 at 10.34.45 AM.png)  
    where:
    
    <table class="" style="table-layout: fixed;"><thead class="" style=""><tr class="" style=""><th class="" style=""><div class="" style="">Field</div></th><th class="" style=""><div class="" style="">Description</div></th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style="">Request Method</td><td class="" style=""><span style="" class="">The request method indicates the expected action to be executed on the specified resource. Katalon Studio supports following SOAP methods: SOAP, SOAP 1.2, POST, GET.</span></td></tr><tr class="" style=""><td class="" style="">Request URL</td><td class="" style="">The WSDL address registered for the SOAP web service.</td></tr><tr class="" style=""><td class="" style="">Service Function</td><td class="" style=""><div class="" style=""><p class="" style="">The function/method of the SOAP web service that you want to use in this SOAP request. The list will be retrieved after clicking&nbsp;<strong class="" style="">Load from WSDL</strong>. <span class="" style=""><img class="" height="250" src="../../images/katalon-studio/docs/soap-latest/Screen Shot 2018-04-05 at 10.40.05 AM.png" data-image-src="/download/attachments/13697583/Screen%20Shot%202018-04-05%20at%2010.40.05%20AM.png?version=1&amp;modificationDate=1522899637000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="13697838" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="Screen Shot 2018-04-05 at 10.40.05 AM.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="13697583" data-linked-resource-container-version="3" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style="">Authorization</td><td class="" style=""><div class="" style=""><p class="" style="">Credential for HTTP authentication.</p><p class="" style=""><span class="" style=""><img class="" height="150" src="../../images/katalon-studio/docs/soap-latest/Screen Shot 2018-04-05 at 10.37.05 AM.png" data-image-src="/download/attachments/13697583/Screen%20Shot%202018-04-05%20at%2010.37.05%20AM.png?version=1&amp;modificationDate=1522899442000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="13697836" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="Screen Shot 2018-04-05 at 10.37.05 AM.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="13697583" data-linked-resource-container-version="3" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style="">HTTP Headers</td><td class="" style=""><div class="" style=""><p class="" style="">The header information that you want to transmit in this SOAP request object.</p><p class="" style="">You can select headers from the list of suggested options (by double-clicking on the&nbsp;<strong class="" style="">Name</strong>&nbsp;cell) or enter another header of your interest. Refer to&nbsp;<a class="" href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers" rel="nofollow" style="">Supported HTTP Headers</a>&nbsp;for more details.</p><p class="" style=""><span class="" style=""><img class="" height="250" src="../../images/katalon-studio/docs/soap-latest/Screen Shot 2018-04-05 at 10.39.09 AM.png" data-image-src="/download/attachments/13697583/Screen%20Shot%202018-04-05%20at%2010.39.09%20AM.png?version=1&amp;modificationDate=1522899567000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="13697837" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="Screen Shot 2018-04-05 at 10.39.09 AM.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="13697583" data-linked-resource-container-version="3" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style="">Request Message</td><td class="" style=""><div class="" style=""><p class="" style="">The information that you want to transmit in this SOAP request object.&nbsp;You can enter directly or import content from external text files.&nbsp;</p><p class="" style=""><span class="" style=""><img class="" height="250" src="../../images/katalon-studio/docs/soap-latest/Screen Shot 2018-04-05 at 10.41.28 AM.png" data-image-src="/download/attachments/13697583/Screen%20Shot%202018-04-05%20at%2010.41.28%20AM.png?version=2&amp;modificationDate=1522900253000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="13697839" data-linked-resource-version="2" data-linked-resource-type="attachment" data-linked-resource-default-alias="Screen Shot 2018-04-05 at 10.41.28 AM.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="13697583" data-linked-resource-container-version="3" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style="">Response</td><td class="" style=""><div class="" style=""><p class="" style="">The retrieved message from web service server when you click&nbsp;<strong class="" style="">Test Request </strong>button. You can view details information of the response including <strong class="" style="">Status</strong>, <strong class="" style="">Elapsed Time</strong>, <strong class="" style="">Size.</strong></p><p class="" style="">There are 2 viewing format: <strong class="" style="">pretty</strong> or <strong class="" style="">raw</strong></p><p class="" style=""><span class="" style=""><img class="" height="250" src="../../images/katalon-studio/docs/soap-latest/Screen Shot 2018-04-05 at 10.50.38 AM.png" data-image-src="/download/attachments/13697583/Screen%20Shot%202018-04-05%20at%2010.50.38%20AM.png?version=1&amp;modificationDate=1522900319000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="13697841" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="Screen Shot 2018-04-05 at 10.50.38 AM.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="13697583" data-linked-resource-container-version="3" style=""></span> <span class="" style=""><img class="" width="353" src="../../images/katalon-studio/docs/soap-latest/Screen Shot 2018-04-05 at 10.52.27 AM.png" data-image-src="/download/attachments/13697583/Screen%20Shot%202018-04-05%20at%2010.52.27%20AM.png?version=1&amp;modificationDate=1522900390000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="13697842" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="Screen Shot 2018-04-05 at 10.52.27 AM.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="13697583" data-linked-resource-container-version="3" style=""></span></p><p class="" style="">&nbsp;</p></div></td></tr></tbody></table>
    
4.  Save the service request object when you're done. The service request defined here can be utilized in other test cases. Refer to [Use Web Service in Test Case](/display/KD/Using+Web+Service+in+Test+Case) for more details.