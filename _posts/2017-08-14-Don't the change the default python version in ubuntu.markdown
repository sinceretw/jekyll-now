---
layout: post
title:  "Don't change the default python version in ubuntu"
date:   2017-08-14 12:09:26 -0500
categories: ubuntu
---
Don't change the default python version (python 2) in ubuntu to the last version (python 3), or else, apt-get install/update wouldn't function correclly. All kinds of errors would came out.

(Reading database ... 367898 files and directories currently installed.)
Preparing to unpack .../python-libxml2_2.9.3+dfsg1-1ubuntu0.2_amd64.deb ...
  File "/usr/bin/pyclean", line 63
    except (IOError, OSError), e:
                             ^
SyntaxError: invalid syntax

user python -V check the default version, if it shows 3.*.*, then change it back use the following command
sudo ln -s /user/bin/python2.7 /user/bin/python.

Spend two days to resolve the error when try to install nginx in ubuntu, have tried all the possible solution from online, and finally found out the python version issue.


不要改变ubuntu中的默认python版本（2.7），为了方便把默认的python版本从2改称3了，在用apt-get安装nginx时遇到各种各样的错误，花了两天时间才算找到原因。
 
