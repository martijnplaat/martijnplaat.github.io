---
layout: post-light-feature
title: "Rule of the least power"
description: "Keep your data on the web open by using a hybrid model of descriptive-, declaritive- and turing-complete languages"
categories: articles
date: 2015-07-03
tags: [javascript, programming, atwood]
comments: true
image:
	feature: http://farm9.staticflickr.com/8426/7758832526_cc8f681e48_c.jpg
---

@angular_nu: "Not sure WebAssembly http://ow.ly/OwDNW  is going to make it as it violates Atwood's law: http://ow.ly/OwDXx . #webassemby #javascript"

I read this tweet recently. 

Since I have my background in semantic web technologies I have to say that we can only leverage the power of the web when data is freely available for everyone and even more; computers should be able to interpret the meaning of this data. The web, as we notice today, holds data which is freely available but, the semantics of the data is still locked up in our back-end databases. This lack of semantics on the web is not the point I want to make and is still a shortcoming of the web we hopefully overcome somewhere in the near future.

But, what we have accomplished, is a web of connected documents with open -freely available- data which could be indexed and analysed by search engines and advanced web applications. In my opinion there are two trends that threatens this powerful foundation.

The first threat is hidden in Atwood's Law;

```
"Any application that can be written in Javascript, will eventually be written in Javascript"
```

Should we Javascript all things?

<figure>
	<img src="http://www.quickmeme.com/img/8d/8d30a19413145512ad5a05c46ec0da545df5ed79e113fcf076dc03c7514eb631.jpg">
</figure>

No not really. Remember when building web applications; "Declaritive First". This is really important because with a declaritive language the data can be used far beyond an individual implementation.

```
"An imperative-only JavaScript web is enticing if we understand the web as open technologies and connected documents. But if we expand our understanding of the web to include connected systems, then declarative programming is a key part of how we connect those systems."
``` -- [Declarative Programming And The Web by Scot Reynen](http://www.smashingmagazine.com/2014/07/30/declarative-programming/)

The second threat is actually where the mentioned tweet is all about. What we try to accomplish with WebAssembly is an invitation on the web of really powerful imperative languages like C, C++, etc.

Now what the [Rule Of The Least Power](http://www.w3.org/2001/tag/doc/leastPower.html) actually says is that when you choose a language to process your data, especially when this data is published on the web, you should start with a language with the least power.
Since the least powerful languages intrinsically facilitate the data in their language to web developers on the World Wide Web. Ie. we should advocate open data on the web, and therefore be aware of locking up the data in our programming languages!

Respectively from least powerful to powerful we distinguest the following type of languages: descriptive languages (XML, HTML, RDF), limited propositional logic (access control lists, regular expressions) , declarative languages (JSON, SQL, XST, OWL), functional languages (Hashkell, Javascript) and finally imperative and turing-complete languages (Java, C, JavaScript).

Thus, I do not say that we should not use Javascript and WebAssembly but, when building a website/webapplication you should use a layered model and start with exposing your data in a descriptive language up to maybe even the use of C++ within a WebAssembly implementation :)







