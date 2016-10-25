---
layout: post
title: "Frameworks of ntop"
date: 2016-10-26
---

Framework of ntopng is really awesome. It has three layers, i.e., ingress layer 
for capture data, monitoring engine for handle data, Lua scripting engine for 
export data to web or third-partis.

The ingress layer can communicate with other nProbe application using ZeroMQ.

The monitor engine is written in C++. And they write some classes for Lua scripting 
enging using C++. So Lua scripts can call these C++ codes. They also write a HTTPServer 
with C++ to handle http requests. But the content of reponse is handled by Lua scripting 
enging. So the basic process is:

Web browser send http requests to C++ http server. Http server catch a request, 
parse it, and call related Lua scripts to generate response content. Then Lua script 
calls some C++ codes and generate html code.

Awesome! I never thought that they write a C++ HTTP server in ntopng.
