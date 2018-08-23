---
title: "Update or Replace Web Browser Drivers and Selenium" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/update-or-replace-web-browser-drivers-and-selenium.html 
description: 
---
For manually replacing and updating other versions of WebDrivers and Selenium, please refer to this [guide](https://docs.katalon.com/x/1xtO). 

Katalon Studio team strongly suggest users **NOT** to manually replace or update any WebDrivers. Any changes in drivers may cause runtime bugs for Katalon Studio application.

<table class="" style="table-layout: fixed;"><thead><tr><th class="" style="">Katalon Studio V5.1.0</th><th class="" colspan="2" style="">How to Replace&nbsp;</th></tr></thead><tbody class="" style=""><tr class="" style=""><td class="" colspan="1" style="">&nbsp;</td><td class="" data-highlight-colour="grey" style=""><strong class="" style="">Windows</strong></td><td class="" data-highlight-colour="grey" style=""><strong class="" style="">MAC OSX</strong></td></tr><tr class="" style=""><td class="" style="">Selenium <a class="" href="https://raw.githubusercontent.com/SeleniumHQ/selenium/master/java/CHANGELOG" rel="nofollow" style="">3.7.1</a></td><td class="" colspan="1" style=""><ul class="" style=""><li class="" style=""><strong class="" style="">Download </strong>the desired Selenium version <a class="" href="http://selenium-release.storage.googleapis.com/index.html" rel="nofollow" style="">here</a> (<span class="" style="">Select </span><strong class="" style="">only</strong><span class="" style=""> Selenium 3.0+ and higher version than 3.7.1)</span></li><li class="" style=""><span class="" style=""><strong class="" style="">Delete</strong> existing selenium-server-standalone-3.x.jar</span><span class="" style=""><br class="" style=""></span></li><li class="" style=""><span class="" style=""><strong class="" style="">Copy</strong> preferred <strong class="" style="">driver</strong> into this folder</span><br class="" style="">&lt;Katalon Studio folder&gt;\configuration\resources\lib</li></ul></td><td class="" colspan="1" style=""><p class="" style="">&nbsp;</p><ul class="" style=""><li class="" style="">&nbsp;/Applications/Katalon Studio.app/Contents/Eclipse/configuration/resources/lib</li></ul></td></tr><tr class="" style=""><td class="" style="">Chromedriver <a class="" href="https://chromedriver.storage.googleapis.com/2.33/notes.txt" rel="nofollow" style="">2.33</a></td><td class="" colspan="1" style=""><div class="" style=""><ul class="" style=""><li class="" style=""><strong class="" style="">Download </strong>preferred Chromedriver <a class="" href="https://sites.google.com/a/chromium.org/chromedriver/downloads" rel="nofollow" style="">here</a></li><li class="" style=""><strong class="" style="">Copy</strong> downloaded Chromedriver and <strong class="" style="">paste</strong> into Katalon Studio folder</li></ul><div class="" data-hasbody="true" data-macro-name="info" style=""><span class="" style=""></span><div class="" style=""><p class="" style="">You can use 32-bit Windows Chromedriver for both 32-bit and 64-bit Windows.</p></div></div><ul class="" style=""><li style="" class=""><ul class="" style=""><li class="" style="">&lt;Katalon Studiofolder&gt;\configuration\resources\drivers\chromedriver_win32</li><li class="" style="">&lt;Katalon Studiofolder&gt;\configuration\resources\drivers\chromedriver_win64</li></ul></li></ul></div></td><td class="" colspan="1" style=""><p class="" style="">&nbsp;</p><ul class="" style=""><li class="" style="">/Applications/Katalon Studio.app/Contents/Eclipse/configuration/resources/drivers/chromedriver_mac</li></ul></td></tr><tr class="" style=""><td class="" style="">Firefox (Gecko Driver) <a class="" href="https://github.com/mozilla/geckodriver/releases/tag/v0.19.0" rel="nofollow" style="">0.19</a></td><td class="" colspan="1" style=""><ul class="" style=""><li class="" style=""><strong class="" style="">Download </strong>preferred Gecko Driver <a class="" href="https://github.com/mozilla/geckodriver/releases" rel="nofollow" style="">here</a><span class="" style=""><strong class="" style=""><br class="" style=""></strong></span></li><li class="" style=""><span class="" style=""><strong class="" style="">Copy</strong><span class="" style=""> downloaded Gecko driver and </span><strong class="" style="">paste</strong><span class="" style=""> into Katalon Studio folder</span></span><ul class="" style=""><li class="" style=""><span class="" style="">&lt;Katalon Studio folder&gt;\configuration\resources\drivers\firefox_win32</span></li><li class="" style="">&lt;Katalon Studio folder&gt;\configuration\resources\drivers\firefox_win64</li></ul></li></ul></td><td class="" colspan="1" style=""><p class="" style="">&nbsp;</p><ul class="" style=""><li class="" style="">/Applications/Katalon Studio.app/Contents/Eclipse/configuration/resources/drivers/firefox_mac</li></ul></td></tr><tr class="" style=""><td class="" colspan="1" style="">IEDriverServer <a class="" href="https://raw.githubusercontent.com/SeleniumHQ/selenium/master/cpp/iedriverserver/CHANGELOG" rel="nofollow" style="">3.6.0</a></td><td class="" colspan="1" style=""><ul class="" style=""><li class="" style="">Download preferred IEDriver <a class="" href="http://selenium-release.storage.googleapis.com/index.html" rel="nofollow" style="">here</a></li><li class="" style=""><strong class="" style="">Copy</strong><span class="" style=""> downloaded IEDriverServer and </span><strong class="" style="">paste</strong><span class="" style=""> into Katalon Studio folder</span></li><li class="" style="">&lt;Katalon Studio folder&gt;\configuration\resources\drivers\iedriver_win32</li><li class="" style="">&lt;Katalon Studio folder&gt;\configuration\resources\drivers\iedriver_win64</li></ul></td><td class="" colspan="1" style="">&nbsp;</td></tr></tbody></table>