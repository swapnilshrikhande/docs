---
title: "Control Statements" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/control-statements.html 
description: 
---
Katalon Studio provides the ability to dictate the logical flow of execution by supporting **control statements** such as _If/Else_, _for/while_ or _Try/Catch_… which are very common concepts in programming language.

The following control statements are supported in Katalon Studio:

*   [Decision-making statements](https://docs.katalon.com/display/KD/Control+Statements#ControlStatements-Decision-makingstatements) 
*   [Looping statements](https://docs.katalon.com/display/KD/Control+Statements#ControlStatements-Loopingstatements)
*   [Branching statements](https://docs.katalon.com/display/KD/Control+Statements#ControlStatements-Branchingstatements)
*   [Exception handling block](https://docs.katalon.com/display/KD/Control+Statements#ControlStatements-Exceptionhandlingblock)

Once a test step is added as any of the control statements, it will **not** be allowed to change it into another keyword.

Decision-making statements 
---------------------------

### In Manual view 

Open a test case in **Manual** view, then navigate to **Decision-making Statements** from command toolbar.

![](../../images/katalon-studio/docs/control-statements/image2017-6-30 20_40_1.png)

Refer to the following table for the usage of each statement:

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Statement</th><th class="" style="">Description</th><th class="" style="">Screenshot</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style="">If</td><td class="" style="">This statement requires a <strong class="" style="">boolean condition</strong> as <strong class="" style="">input value</strong>. Katalon Studio will execute all steps within once the condition is triggered.</td><td rowspan="3" class="" style=""><div class="" style=""><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/image2017-2-9 14_23_17.png" data-image-src="/download/attachments/786604/image2017-2-9%2014%3A23%3A17.png?version=1&amp;modificationDate=1486624997000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5112260" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-9 14:23:17.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style="">Else If</td><td class="" style="">Using <strong class="" style="">Else If</strong> after <strong class="" style="">If</strong>, you can create a combination of conditions where the steps within the <em class="" style="">first</em> satisfied condition will be executed.</td></tr><tr class="" style=""><td colspan="1" class="" style="">Else</td><td colspan="1" class="" style="">This statement serves as the conclusion of the <strong class="" style="">If - Else If - Else</strong> structure. The steps within this statement will be executed if <strong class="" style="">all</strong> the conditions above it are <strong class="" style="">not</strong> triggered.</td></tr><tr class="" style=""><td colspan="1" class="" style="">Switch</td><td colspan="1" class="" style="">This statement requires an expression, which is often referred to as <strong class="" style="">the control expression</strong> (or <strong class="" style="">control variable</strong>), as <strong class="" style="">input value</strong>.</td><td rowspan="3" class="" style=""><div class="" style=""><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/image2017-2-9 14_47_59.png" data-image-src="/download/attachments/786604/image2017-2-9%2014%3A47%3A59.png?version=1&amp;modificationDate=1486626480000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5112261" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-9 14:47:59.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr><tr class="" style=""><td colspan="1" class="" style="">Case</td><td colspan="1" class="" style=""><p class="" style="">The <strong class="" style="">Cases</strong> indicate the assumed value for the <strong class="" style="">control expression</strong>, <span style="" class="">with corresponding steps to be executed when a match occurs.</span></p><p class="" style="">Each <strong class="" style="">Case</strong> will have a <strong class="" style="">Break</strong> by default which should be positioned at the end of the <strong class="" style="">Case</strong> block to mark the end of it.</p></td></tr><tr class="" style=""><td colspan="1" class="" style="">Default</td><td colspan="1" class="" style="">This statement is included automatically within every <strong class="" style="">Switch</strong> statement. In situation which <strong class="" style="">no</strong> <strong class="" style="">Case</strong> value can be matched, the steps within <strong class="" style="">Default</strong> will be taken.</td></tr></tbody></table>

### In Scripting view

The **Script** view of test cases allows you to programmatically define and handle **If-ElseIf-Else** or **Switch-Case** structure easily using either Groovy or Java language. Refer to [http://groovy-lang.org/semantics.html#\_conditional\_structures](http://groovy-lang.org/semantics.html#_conditional_structures) for more details about conditional structure in Groovy.

For example:

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Decision-making statement</th><th class="" style="">Screenshot</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style=""><p class="" style="">If - Else If - Else</p></td><td class="" style=""><div class="" style=""><p class="" style="">&nbsp;<span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/10.png" data-image-src="/download/attachments/786604/10.png?version=1&amp;modificationDate=1452064114000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="787287" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="10.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Switch - Case</p></td><td class="" style=""><div class="" style="">&nbsp;<span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/11.png" data-image-src="/download/attachments/786604/11.png?version=1&amp;modificationDate=1452064115000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="787288" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="11.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></div></td></tr></tbody></table>

Looping statements 
-------------------

### In Manual view 

Open a test case in **Manual** view, then navigate to **Looping Statements** from command toolbar.

![](../../images/katalon-studio/docs/control-statements/image2017-6-30 20_40_53.png)

Refer to following table for the usage of each statement:

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Statement</th><th class="" style="">Description</th><th class="" style="">Screenshot</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style="">For</td><td class="" style=""><span class="" style="">This statement accepts a <em class="" style="">range</em>,<em class="" style=""> list</em> or <em class="" style="">array</em> as <strong class="" style="">input value</strong> so that Katalon Studio knows <strong class="" style="">how many times</strong> to execute all steps within the <strong class="" style="">For</strong> structure.</span></td><td class="" style=""><div class="" style=""><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/image2017-2-9 15_49_5.png" data-image-src="/download/attachments/786604/image2017-2-9%2015%3A49%3A5.png?version=1&amp;modificationDate=1486630146000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5112268" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-9 15:49:5.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style="">While</td><td class="" style=""><span class="" style="">This statement requires a <strong class="" style="">boolean condition</strong> as <strong class="" style="">input value</strong> so that Katalon Studio will keep executing all steps within <strong class="" style="">until the condition fails</strong>.</span></td><td class="" style=""><div class="" style=""><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/image2017-2-9 15_53_44.png" data-image-src="/download/attachments/786604/image2017-2-9%2015%3A53%3A44.png?version=1&amp;modificationDate=1486630424000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5112269" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-9 15:53:44.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr></tbody></table>

### In Scripting view 

The **Script** View of test cases allows you to programmatically define and handle **For** or **While** structure easily using either Groovy or Java language. Refer to [http://groovy-lang.org/semantics.html#\_looping\_structures](http://groovy-lang.org/semantics.html#_looping_structures) for more details about looping structures in Groovy.

For example:

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Looping statement</th><th class="" style="">Screenshot</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style=""><p class="" style="">For</p></td><td class="" style=""><div class="" style=""><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/24.png" data-image-src="/download/attachments/786604/24.png?version=1&amp;modificationDate=1452064128000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="787301" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="24.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">While</p></td><td class="" style=""><div class="" style=""><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/25.png" data-image-src="/download/attachments/786604/25.png?version=1&amp;modificationDate=1452064129000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="787302" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="25.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr></tbody></table>

Branching statements 
---------------------

### In Manual view 

Open a test case in **Manual** view, then navigate to **Branching Statements** from command toolbar.

![](../../images/katalon-studio/docs/control-statements/image2017-6-30 20_41_31.png)

Refer to following table for the usage of each statement:

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Statement</th><th class="" style="">Description</th><th class="" style="">Screenshot</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style="">Break</td><td class="" style=""><p class="" style="">Katalon Studio will exit current code block and continue to next code block / test step.</p></td><td class="" style=""><div class="" style=""><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/image2017-2-9 16_36_37.png" data-image-src="/download/attachments/786604/image2017-2-9%2016%3A36%3A37.png?version=1&amp;modificationDate=1486632997000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5112272" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-9 16:36:37.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style="">Continue</td><td class="" style=""><span style="" class="">Katalon Studio will skip the remainder of the current loop and continue with the next iteration of the loop.</span></td><td class="" style=""><div class="" style=""><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/image2017-2-9 16_42_13.png" data-image-src="/download/attachments/786604/image2017-2-9%2016%3A42%3A13.png?version=1&amp;modificationDate=1486633334000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5112273" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-9 16:42:13.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr><tr class="" style=""><td class="" style="">Return</td><td class="" style=""><span style="" class="">Katalon will exit from the current method/step, and the flow control is returned to where the method/step was invoked.</span></td><td class="" style=""><div class="" style=""><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/image2017-2-9 16_47_44.png" data-image-src="/download/attachments/786604/image2017-2-9%2016%3A47%3A44.png?version=1&amp;modificationDate=1486633665000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5112274" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-9 16:47:44.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr></tbody></table>

### In Scripting view

The **Script** view of test cases allows you to programmatically define and handle **Break**, **Continue** & **Return** easily using either Groovy or Java language. 

For example:

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Decision-making statement</th><th class="" style="">Screenshot</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style=""><p class="" style="">Break</p></td><td class="" style=""><div class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/36.png" data-image-src="/download/attachments/786604/36.png?version=1&amp;modificationDate=1452064141000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="787313" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="36.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></div></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Continue</p></td><td class="" style=""><div class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/37.png" data-image-src="/download/attachments/786604/37.png?version=1&amp;modificationDate=1452064142000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="787314" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="37.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></div></td></tr><tr class="" style=""><td class="" style=""><p class="" style="">Return</p></td><td class="" style=""><div class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/38.png" data-image-src="/download/attachments/786604/38.png?version=1&amp;modificationDate=1452064142000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="787315" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="38.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></div></td></tr></tbody></table>

Exception handling block 
-------------------------

### In Manual view 

Open a test case in **Manual** view, then navigate to **Exception Handling Statements** from command toolbar.

![](../../images/katalon-studio/docs/control-statements/image2017-6-30 20_42_21.png)

Refer to following table for the usage of each statement:

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Statement</th><th class="" style="">Description</th><th class="" style="">Screenshot</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" style="">Try</td><td class="" style="">This statement indicates that all steps within will be monitored by<span style="" class=""><strong class="" style=""> exception handlers</strong>.</span></td><td rowspan="4" class="" style=""><div class="" style=""><p class="" style=""><span class="" style=""><img class="" src="../../images/katalon-studio/docs/control-statements/image2017-2-28 11_51_55.png" data-image-src="/download/attachments/786604/image2017-2-28%2011%3A51%3A55.png?version=1&amp;modificationDate=1488257515000&amp;api=v2" data-unresolved-comment-count="0" data-linked-resource-id="5113399" data-linked-resource-version="1" data-linked-resource-type="attachment" data-linked-resource-default-alias="image2017-2-28 11:51:55.png" data-base-url="https://docs.katalon.com" data-linked-resource-content-type="image/png" data-linked-resource-container-id="786604" data-linked-resource-container-version="1" style=""></span></p></div></td></tr><tr class="" style=""><td colspan="1" class="" style="">Throw</td><td colspan="1" class="" style="">Before you can <strong class="" style="">Catch</strong> an exception, some code must throw one. Regardless of what throws the exception, it's always involved with the <strong class="" style="">Throw</strong> statement</td></tr><tr class="" style=""><td class="" style="">Catch</td><td class="" style=""><span class="" style="">Katalon Studio will&nbsp;</span><span style="" class="">execute all steps within when there is any issue occurred during execution of the <strong class="" style="">Try</strong> block.</span></td></tr><tr class="" style=""><td class="" style="">Finally</td><td class="" style="">This is the last part of the <strong class="" style="">Try-Catch-Finally</strong> structure and <span style="" class="">all steps within this will be executed regardless of any exception.</span></td></tr></tbody></table>

### In Scripting view

The **Script** view of test cases allows you to programmatically define and handle exception easily using either Groovy or Java language. Refer to [http://groovy-lang.org/semantics.html#\_try\_catch_finally](http://groovy-lang.org/semantics.html#_try_catch_finally) for more details about exception handling in Groovy.

For example:

![](../../images/katalon-studio/docs/control-statements/image2017-2-28 13_20_32.png)