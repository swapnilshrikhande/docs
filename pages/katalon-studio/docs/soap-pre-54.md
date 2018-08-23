---
title: "SOAP (Pre-5.4)" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/soap-pre-54.html 
description: 
---
Create SOAP Object
------------------

1.  Select **File > New > Web Service Request** from the main menu. The **New Web Service Request** dialog will be displayed.  
    ![](../../images/katalon-studio/docs/soap-pre-54/image2017-2-13 14_4_53.png)  
    Provide the name for the new service request object, select **SOAP** as **Request Type** then click **OK**.  
      
    
2.  A new service request object is created under **Object Repository** of Katalon Studio.  
    ![](../../images/katalon-studio/docs/soap-pre-54/image2017-2-13 14_5_47.png)  
      
    
3.  In the opened editor of the new service request object, enter all required information.  
    ![](../../images/katalon-studio/docs/soap-pre-54/image2017-6-30 20_48_48.png)  
    where:
    
    <table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Field</th><th class="" style="">Description</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style="">Request Method</td><td class="" style=""><span style="" class="">The request method indicates the expected action to be executed on the specified resource. Katalon Studio supports following SOAP methods: SOAP, SOAP 1.2, POST, GET.</span></td></tr><tr class="" style=""><td class="" style="">Request URL</td><td class="" style=""><span class="" style="">The WSDL address registered for the SOAP web service.</span></td></tr><tr class="" style=""><td class="" style="">Service Function</td><td class="" style=""><span class="" style="">The function/method of the SOAP web service that you want to use in this SOAP request. The list will be retrieved after clicking <strong class="" style="">Load from WSDL</strong>.</span></td></tr><tr class="" style=""><td class="" style="">Authorization</td><td class="" style=""><div class="" style=""><p class="" style="">Credential for HTTP authentication.</p><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/soap-pre-54/image2017-2-13 13_31_8.png" data-image-src="/download/attachments/5116882/image2017-2-13%2013%3A31%3A8.png?version=1&amp;modificationDate=1503888061000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5116896" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-13 13:31:8.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="5116882" data-linked-resource-container-version="1" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style="">HTTP Headers</td><td class="" style=""><div class="" style=""><p class="" style="">The header information that you want to transmit in this SOAP request object.</p><p class="" style=""><span class="" style=""><span class="" style="">You can select headers from the list of suggested options (by double clicking on the </span><strong class="" style="">Name</strong><span class="" style=""> cell) or enter another header of your interest</span>. Refer to&nbsp;<a href="#SOAP(Pre-5.4)-SupportedHTTPHeaders" class="" style="">Supported HTTP Headers</a></span><span class="" style="">&nbsp;for more details.</span></p><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/soap-pre-54/image2017-2-13 13_33_57.png" data-image-src="/download/attachments/5116882/image2017-2-13%2013%3A33%3A57.png?version=1&amp;modificationDate=1503888061000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5116897" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-13 13:33:57.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="5116882" data-linked-resource-container-version="1" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style="">Request Message</td><td class="" style=""><div class="" style=""><p class="" style=""><span class="" style="">The information that you want to transmit in this SOAP request object. <span class="" style="">You can enter directly or import content from external text files. </span><span class="" style=""><img class="" src="../../images/katalon-studio/docs/soap-pre-54/image2017-2-13 14_20_16.png" data-image-src="/download/attachments/5116882/image2017-2-13%2014%3A20%3A16.png?version=1&amp;modificationDate=1503888061000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5116898" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-13 14:20:16.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="5116882" data-linked-resource-container-version="1" style=""></span></span></p></div></td></tr><tr class="" style=""><td class="" style="">Response</td><td class="" style=""><div class="" style=""><p class="" style=""><span class="" style="">The retrieved message from web service server when you click <strong class="" style="">Test Request</strong>.</span></p><p class="" style=""><span class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/soap-pre-54/image2017-2-13 14_21_55.png" data-image-src="/download/attachments/5116882/image2017-2-13%2014%3A21%3A55.png?version=1&amp;modificationDate=1503888061000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5116899" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-13 14:21:55.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="5116882" data-linked-resource-container-version="1" style=""></span></span></p></div></td></tr></tbody></table>
    
4.  Save the service request object when you're done. The service request defined here can be utilized in other test cases. Refer to [Use WebService in Test Case](#SOAP(Pre-5.4)-UseWebServiceinTestCase) for more details.

Supported HTTP Headers 
-----------------------

Here’s the list of HTTP headers initially supported in Katalon Studio:

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Header field name</th><th class="" style="">Description</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style=""><p class="" style="">Accept</p></td><td class="" style=""><p class="" style="">Content-Type items acceptable for the response.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Accept-Charset</p></td><td class="" style=""><p class="" style="">Character sets that are acceptable.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Accept-Encoding</p></td><td class="" style=""><p class="" style="">List of acceptable encodings.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Accept-Language</p></td><td class="" style=""><p class="" style="">List of acceptable human languages for response.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Authorization</p></td><td class="" style=""><p class="" style="">Authentication credentials for HTTP authentication.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Cache-Control</p></td><td class="" style=""><p class="" style="">Used to specify directives that must be obeyed by all caching mechanisms along the request-response chain</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Connection</p></td><td class="" style=""><p class="" style="">Control options for the current connection and list of hop-by-hop request fields.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Content-Length</p></td><td class="" style=""><p class="" style="">The length of the request body in octets (8-bit bytes)</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Content-Type</p></td><td class="" style=""><p class="" style="">The MIME type of the body of the request (used with POST and PUT requests).</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Cookie</p></td><td class="" style=""><p class="" style="">An HTTP cookie previously sent by the server with Set-Cookie.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">DNT</p></td><td class="" style=""><p class="" style="">Requests a web application to disable their tracking of a user. This is Mozilla's version of the X-Do-Not-Track header field (since Firefox 4.0 Beta 11). Safari and IE9 also have support for this field.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Date</p></td><td class="" style=""><p class="" style="">The date and time that the message was sent (in "HTTP-date" format as defined by RFC 7231 Date/Time Formats.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Expect</p></td><td class="" style=""><p class="" style="">Indicates that particular server behaviors are required by the client.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">From</p></td><td class="" style=""><p class="" style="">The email address of the user making the request.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Front-End-Https</p></td><td class="" style=""><p class="" style="">Non-standard header field used by Microsoft applications and load-balancers.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Host</p></td><td class="" style=""><p class="" style="">The domain name of the server (for virtual hosting), and the TCP port number on which the server is listening. The port number may be omitted if the port is the standard port for the service requested. Mandatory since HTTP/1.1.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">If-Match</p></td><td class="" style=""><p class="" style="">Only perform the action if the client supplied entity matches the same entity on the server. This is mainly for methods like PUT to only update a resource if it has not been modified since the user last updated it.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">If-Modified-Since</p></td><td class="" style=""><p class="" style="">Allows a 304 Not Modified to be returned if content is unchanged.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">If-None-Match</p></td><td class="" style=""><p class="" style="">Allows a 304 Not Modified to be returned if content is unchanged.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">If-Range</p></td><td class="" style=""><p class="" style="">If the entity is unchanged, send me the part(s) that I am missing; otherwise, send me the entire new entity.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">If-Unmodified-Since</p></td><td class="" style=""><p class="" style="">Only send the response if the entity has not been modified since a specific time.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Max-Forwards</p></td><td class="" style=""><p class="" style="">Limit the number of times the message can be forwarded through proxies or gateways.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Origin</p></td><td class="" style=""><p class="" style="">Initiates a request for cross-origin resource sharing (asks server for an 'Access-Control-Allow-Origin' response field).</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Pragma</p></td><td class="" style=""><p class="" style="">Implementation-specific fields that may have various effects anywhere along the request-response chain.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Proxy-Authorization</p></td><td class="" style=""><p class="" style="">Authorization credentials for connecting to a proxy.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Proxy-Connection</p></td><td class="" style=""><p class="" style="">Implemented as a misunderstanding of the HTTP specifications. Common because of mistakes in implementations of early HTTP versions. Has exactly the same functionality as standard Connection field.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Range</p></td><td class="" style=""><p class="" style="">Request only part of an entity. Bytes are numbered from 0.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Referer</p></td><td class="" style=""><p class="" style="">This is the address of the previous web page from which a link to the currently requested page was followed. (The word “referrer” has been misspelled in the RFC as well as in most implementations to the point that it has become standard usage and is considered correct terminology).</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">TE</p></td><td class="" style=""><p class="" style="">The transfer encodings the user agent is willing to accept: the same values as for the response header field Transfer-Encoding can be used, plus the "trailers" value (related to the "chunked" transfer method) to notify the server it expects to receive additional fields in the trailer after the last, zero-sized, chunk.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Upgrade</p></td><td class="" style=""><p class="" style="">Ask the server to upgrade to another protocol.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">User-Agent</p></td><td class="" style=""><p class="" style="">The user agent string of the user agent.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Via</p></td><td class="" style=""><p class="" style="">Informs the server of proxies through which the request was sent.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Warning</p></td><td class="" style=""><p class="" style="">A general warning about possible problems with the entity body.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">X-ATT-DeviceId</p></td><td class="" style=""><p class="" style="">Allows easier parsing of the MakeModel/Firmware that is usually found in the User-Agent String of AT&amp;T Devices</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">X-Csrf-Token</p></td><td class="" style=""><p class="" style="">Used to prevent cross-site request forgery. Alternative header names are: X-CSRFToken and X-XSRF-TOKEN.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">X-Forwarded-For</p></td><td class="" style=""><p class="" style="">A de facto standard for identifying the originating IP address of a client connecting to a web server through an HTTP proxy or load balancer.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">X-Forwarded-Host</p></td><td class="" style=""><p class="" style="">A de facto standard for identifying the original host requested by the client in the Host HTTP request header, since the host name and/or port of the reverse proxy (load balancer) may differ from the origin server handling the request.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">X-Forwarded-Proto</p></td><td class="" style=""><p class="" style="">A de facto standard for identifying the originating protocol of an HTTP request, since a reverse proxy (or a load balancer) may communicate with a web server using HTTP even if the request to the reverse proxy is HTTPS. An alternative form of the header (X-ProxyUser-Ip) is used by Google clients talking to Google servers.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">X-Http-Method-Override</p></td><td class="" style=""><p class="" style="">Requests a web application override the method specified in the request (typically POST) with the method given in the header field (typically PUT or DELETE). Can be used when a user agent or firewall prevents PUT or DELETE methods from being sent directly (note that this either a bug in the software component, which ought to be fixed, or an intentional configuration, in which case bypassing it may be the wrong thing to do).</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">X-Requested-With</p></td><td class="" style=""><p class="" style="">Mainly used to identify Ajax requests. Most JavaScript frameworks send this field with value of XMLHttpRequest.</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">X-UIDH</p></td><td class="" style=""><p class="" style="">Server-side deep packet insertion of a unique ID identifying customers of Verizon Wireless; also known as "perma-cookie" or "supercookie".</p></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">X-Wap-Profile</p></td><td class="" style=""><p class="" style="">Links to an XML file on the Internet with a full description and details about the device currently connecting. In the example to the right is an XML file for an AT&amp;T Samsung Galaxy S2.</p></td></tr></tbody></table>

Refer to [https://en.wikipedia.org/wiki/List\_of\_HTTP\_header\_fields](https://en.wikipedia.org/wiki/List_of_HTTP_header_fields) for more info.