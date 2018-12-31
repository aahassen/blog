+++
type = "post"
author = "Ahmedin Hassen"
date = "2017-06-22"
title = "Angular UI - A Simple Document Management System"
description = ""
featured = ""
featuredpath = ""
featuredalt = ""
categories = ["Angular"]
linktitle = ""
format = "Java"
link = "#"
+++

In this tutorial we will build an Angular UI project for Simple Document Managment System where we can upload, download, update and delete documents and document metadata. This project will use a Spring Boot backend microservice [link to bankend service]. The backend service will provide CRUD functionality for a document. 
This is what the UI look like. The code can be found on the [github](https://github.com/aahassen/DMS-UI)
  ![DMS UI](/img/dms-ui.jpg)
##Lets build the angular-ui
_note that this first you need to run the backend(spring-boot api found here). Becuase this angular project will consume services offered by the backend services..._
We will use the angular-cli commandline framework to create our project. The angular-cli is a framework that allows us to create and manage angular projects and help create the project skeleton help us maintain a common pattern across our application. Run the following commands to create our new angular project. 
``` ng new DMS-UI
    cd DMS-UI
    ng serve
    access localhost:4200
```
Now, if you access [http://localhost:4200](http://localhost:4200) the browser should load the dummy page.

This document management application is composed of the following components/services:
 1. The User Interface module, angular2 application
 2. Doument-service: Microservice built using Spring Boot framework. This service provide CRUD operations on documents
 3. S3-Service: A Microservice that uploads and download document to AWS S3 bucket
 4. Notification-service: Another microservice that will provide a notification service(SMS and Email)

 ## Building the User Interface.
 We are going to use angular CLI to build the UI.
 #Put instruction how to install the CLI
 To create the project, run the following commands in the command line:
 `ng new DMS-UI`
This command will create 