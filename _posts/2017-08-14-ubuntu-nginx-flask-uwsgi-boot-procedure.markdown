---
layout: post
title:  "Ubuntu Nginx Flask Uwsgi boot precdure"
date:   2017-08-18 17:31:26 -0500
categories: ubuntu
---
1. Nginx: sudo service nginx start
2. virtualenv: source activate
3. uwsgi --ini *_uwsgi.ini 

Whenever the html or python code is modified, uwsgi needs to be restarted, if not, the change would not shown on browser.
nginx don't need to resart.

