---
title: "Simple HTTP client "
date: 2020-02-02
tags: [C, UNIX, Networking]
header:
  image: "/images/perceptron/percept.jpg"
excerpt: "C, UNIX, Networking"
mathjax: "true"
---

# Simple HTTP Client

A lightweight CLI HTTP client for academic purposes.

## Features

  - HTTP 0.9, HTTP 1.0, HTTP 1.1 and HTTP 2.0 
  - Based on popular RFC

To run:
```
$ ./client.c
```

What about a [link](https://github.com/)?

C code block:
```c
#include <stdio.h>
#include <errno.h>
#include <unistd.h>
#include <sys/socket.h>
#include <netinet/in.h>
#include <netinet/ip.h>

int main(){
  return 0;
}
```

Here's some inline code `x+y`.

Here's an image:
<img src="{{ site.url }}{{ site.baseurl }}/images/perceptron/linsep.jpg" alt="linearly separable data">

Here's another image using Kramdown:
![alt]({{ site.url }}{{ site.baseurl }}/images/perceptron/linsep.jpg)

Here's some math:

$$z=x+y$$

You can also put it inline $$z=x+y$$
