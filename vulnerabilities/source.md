Auditing Source Code

This module is about getting familiar with vulnerabilities that manifest in applications that compile to native code. An accurate and complete understanding of an application written in a compiled language cannot be achieved without learning about how the compiler transforms source to machine code and how processors execute that code. An easy way to gain experience with these transforms is by reverse engineering compiled variants of your own code or of projects with source code available. At the end of this module you will be able to identify vulnerabilities in compiled languages like C and C++.

Vulnerabilities are commonly identified in large software packages due to their use of third-party software libraries. Common examples include libraries like libxml, libpng, libpoppler, and libfreetype that parse complicated file formats and protocols. Each of these libraries have historically been prone to software flaws that make the applications using them vulnerable to attack. It doesn't help that most software packages fail to update these libraries when new versions come out, making it significant easier to find known vulnerabilities to apply in these cases.

## Lecture

* [Source Code Auditing I](http://vimeo.com/30001189)
* [Source Code Auditing II](http://vimeo.com/29702192)

## 



