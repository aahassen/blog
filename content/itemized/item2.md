+++
type = "itemized"
author = "Ahmedin Hassen"
date = "2017-06-22"
title = "A High Level Overview of the Document Managment System"
description = "We are going to build a Document Management System usining the Microservices Architectural Style "
featured = ""
featuredpath = ""
featuredalt = ""
categories = ["General"]
linktitle = ""
format = "Java"
link = "#"
+++

## Introduction
We are going to build a Document Management System (we will call it DMS going forward) using a microservice architectural style. 
This is what we are going to build <br>
![Document Management System](/img/dms.jpg)
<br>
This is high-level architecture of our system <br>
![GitHub Logo](/img/hl-diagram.jpg)

So now you are existed about what we are going to build, right? if you are not exited we are actually setting up CI/CD pipline, we will dockerize each service and we will setup ELK(application monitoring) we will also be deploying our services on AWS and we will make code change and we will watch our application updated live on production. How about now?
<br>

Alright, before we dive into building our application, lets understand what microservice architectural style is and why it is so good.
<br>

I know you are screaming to see what the code looks like... but, trust me the fundamental is much imortant than the code... code is everywhere and if your really understnad the fundametals you dont need somebody elses code you can just right it. So, just be patience. 

Lets see a couple common of architectural style:

1. The defato one

The most common architecture pattern is the layered architecture pattern, otherwise known as the n-tier architecture pattern. This pattern is the de facto standard for most Java EE applications and therefore is widely known by most architects, designers, and devel‐ opers. The layered architecture pattern closely matches the tradi‐ tional IT communication and organizational structures found in most companies, making it a natural choice for most business appli‐ cation development efforts.

``` java
 @Override
    public void channelInactive(ChannelHandlerContext ctx){
        Assert.notNull(this.channelRepository, "[Assertion failed] - ChannelRepository is required; it must not be null");
        Assert.notNull(ctx);

        String channelKey = ctx.channel().remoteAddress().toString();
        this.channelRepository.remove(channelKey);

        logger.debug("Binded Channel Count is " + this.channelRepository.size());
    }

    public void setChannelRepository(ChannelRepository channelRepository) {
        this.channelRepository = channelRepository;
    }
```




