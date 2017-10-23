# curl Cheat Sheet
[Official man page](https://curl.haxx.se/docs/manpage.html)  
[Official FAQ] (https://curl.haxx.se/docs/faq.html)

---

Jump to: [GET](#get)  | [POST](#post) | [PUT](#put) | [DELETE](#delete) | [PATCH](#patch) | [Verbose Output](#verbose) | [Basic Auth](#basicAuth) | [Ignore Insecure SSL Connections](#insecure) | [Headers](#headers) | [Output to File](#output)

------

##### <a name="get"></a> GET
Example: ```curl http://www.example.com/resource/123```

------

##### <a name="post"></a> POST
```-X POST -d "bodyContents"```  
```-X POST -d @fileWithBodyContents```  
Example: ```curl -X POST -d "my contents to post" http://www.example.com/doit```

------

##### <a name="put"></a> PUT
```-X PUT -d "bodyContents"```  
```-X PUT -d @fileWithBodyContents```  
Example: ```curl -X PUT -d "my contents to put" http://www.example.com/doit```

------

##### <a name="delete"></a> DELETE
```-X DELETE```  
Example: ```curl -X DELETE http://www.example.com/resource/123```

------

##### <a name="patch"></a> PATCH
```--request PATCH -d "patchContents"```  
```--request PATCH -d @fileWithPatchContents```  
Example: ```curl --request PATCH -d "foo=bar" http://www.example.com/resource/123```

------

##### <a name="verbose"></a> Verbose Output
```-v, --verbose```  
Example: ```curl -v https://www.google.com```

------

##### <a name="basicAuth"></a> Basic Auth
```-u username:password```  
Example: ```curl -u claptrap:Password1 http://www.example.com```

------

##### <a name="insecure"></a> Ignore Insecure SSL Connections
```-k, --insecure```  
Example: ```curl -k https://www.badcert.com```

------

##### <a name="headers"></a> Specify Headers
```-H "headerName: headerValue"```  
Example: ```curl -H "Content-Type: application/json" http://www.example.com```

------

##### <a name="output"></a> Write Output to File
```-o, --output <filename>```  
Example: ```curl -o capture.txt http://www.example.com```

