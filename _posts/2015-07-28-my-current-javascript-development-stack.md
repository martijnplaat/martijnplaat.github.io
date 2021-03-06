---
layout: post-light-feature
title: "My current JavaScript development stack"
description: "Angular, ES6, Babel, Browserify, Gulp, Bower, Material, Karma, Jasmine"
categories: articles
date: 2015-07-28
tags: [javascript, programming, assessment, angular]
comments: true
---

Recently, I had to make an assessment for a dutch IT company. Therefore, I made a greenfield Angular-based web-application with all kind of new tools and technologies to build Javascript applications of the future. 

* ECMAScript 6 to prepare myself for the upcoming Angular v2 framework
* BabelJS for transpiling ES6 code into ES5 code
* Browserify to bundle all code into one Javascript file
* Gulp to automatically syntax check-, transpile-, bundle-, and uglify the code
* Bower to manage my static libraries
* NPM package manager to install all kind of packages used in the Gulp task manager
* Angular Material for a slick UI
* Karma and Jasmine for testing the code

The source code for this little application can be found here:

[github.com/martijnplaat/Googlemapapp.git](https://github.com/martijnplaat/googlemapapp.git)

In the particular assessment they gave me an API without Cross-Origin Resource Sharing or any form of API authentication. 
You can test if an API has CORS enabled with the following command:

```
curl -H "Origin: http://www.example.com"   -H "Access-Control-Request-Method: GET"   -H "Access-Control-Request-Headers: X-Requested-With"   -X OPTIONS --verbose http://still-atoll-8938.herokuapp.com/api/locations/streets?q=d&max=20
```

If you see Access-Control-Allow-Origin: * then we know the API supports CORS:

HTTP/1.1 200 OK\\
< Access-Control-Allow-Origin: *\\
< Access-Control-Allow-Methods: GET, POST\\
< Access-Control-Allow-Headers: Content-Type\\
< Access-Control-Max-Age: 86400\\
< Allow: GET, HEAD, POST, TRACE, OPTIONS\\
< Date: Wed, 22 Jul 2015 15:53:12 GMT\\
< Content-Type: text/html\\
* Server Google Frontend is not blacklisted\\
< Server: Google Frontend\\
< Content-Length: 0\\
< Alternate-Protocol: 80:quic,p=0

In the end this crappy API was actually part of the assessment. However, I came with a quick-and-dirty solution to temporarily overcome the CORS shortcoming; simply disable web-security in the Chrome browser:

```
open -a Google\ Chrome --args --disable-web-security
```

Below you can find the presentation I gave to present my web-application:

<iframe src="//slides.com/martijnvanderplaat-1/deck/embed" width="576" height="420" scrolling="no" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

