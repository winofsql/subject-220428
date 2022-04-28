# subject-220428

## Apache httpd.conf 設定
![image](https://user-images.githubusercontent.com/1501327/165674740-70e2521b-5b26-4b01-ad34-f0f5b7a9fbcd.png)

## ソース先頭
```
#!C:\app2\Python\python.exe
```

![image](https://user-images.githubusercontent.com/1501327/165674257-e612b180-7f88-493f-8ca6-895349a3d76a.png)
```py
html_data = html_data.replace("<","&lt;").replace(">","&gt;").replace("\n","<br>")
```
![image](https://user-images.githubusercontent.com/1501327/165674336-24c65a38-554c-439b-8d69-4631ea20371f.png)

## WEBアプリ基本部分
```py
import cgi
import cgitb
cgitb.enable()

import sys
import io
import os
import urllib.parse
from xml.sax.saxutils import *

sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding='utf-8')

print("Content-Type: text/html; charset=utf-8")
print( "Expires: Thu, 19 Nov 1981 08:52:00 GMT" )
print( "Cache-Control: no-store, no-cache, must-revalidate, post-check=0, pre-check=0" )
print( "Pragma: no-cache" )
print()
```

