---
layout: post
title:  "MIME issue with flask or Django web application"
date:   2017-09-07 17:31:26 -0500
categories: python
---
The web app developed with Flask or Django could not display properly in window enviroment while no issue in Mac or Linux.
windows->run->regedit-> delete the key and value related .css in "\HKey_Classses_Root\.css".
Restart the web app, and it should work fine now.

referrence
https://stackoverflow.com/questions/13772884/css-problems-with-flask-web-app

