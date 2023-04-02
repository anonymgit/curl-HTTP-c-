# curl-HTTP-c-
hey folks, this repository contains a simple configuration and implementation of curl in c++ to amke http request in c++.Follow the readme section to setup and use this demo repository.

- **problem statement** - to make http request from c++ to server(eg. localhost:8080/my-endpoint) 
- **solution** -used curl in c++ to make http request.
below is the setup process

# setup this repo
- clone this repo
- open your command prompt
- navigate to folder where you want to copy and,
- clone using command : git clone https://github.com/anonymgit/curl-HTTP-c-.git
- change your end point link and parameter according to your need.
- run your server 
- then run your c++ code.


# setup in your own repo
- download the curl folder from my repo
- curl folder contains folder like(x64 debug,x64 release,x86 debug ,x86 release)
- copy that folder in your project directory,where .cpp file exist.
- include some header file given below:
```
#define CURL_STATICLIB
#include <iostream>
#include <string>
#include "curl/curl.h"

#ifdef _DEBUG
#pragma comment (lib,"curl/libcurl_a_debug.lib")
#else
#pragma comment (lib,"curl/libcurl_a.lib")
#endif

#pragma comment (lib,"Normaliz.lib")
#pragma comment (lib,"Ws2_32.lib")
#pragma comment (lib,"Wldap32.lib")
#pragma comment (lib,"Crypt32.lib")
#pragma comment (lib,"advapi32.lib")
```
- now customize your code according to your need ,pass parameters which you need then run your server and then run your c++ code.

Thanks for visiting.
