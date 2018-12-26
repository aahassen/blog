+++
author = "Ahmedin Hassen"
categories = ["Microservice", "Spring Boot", "Java"]
tags = ["MicroService"]
date = "2018-12-09"
description = "A Simple Document management application build using microservice architectural style."
featured = "pic03.jpg"
featuredalt = "Pic 3"
featuredpath = "date"
linktitle = ""
title = "Inroduction to Microservices"
type = "post"

+++

## Introduction Microservice. 

In this tutorial we are going to learn how to create MicroServices using Spring Boot Framework. An effective way to learn microservices is creating them, for that we are going to build a simple Document Management System using Microservices architecture. This Document Management System has the following functionalities; upload a document(*.pdf, *.doc, *.txt... etc, even *.zip), get list of documents , update a document and delete a document(s). Basically we will be able to do CRUD operations on documents and we will be storing the docs/files on **AWS S3** bucket and storing document metadata associated with the file on **MYSQL** database.
  This is what the UI will look like at the end.
  <br>
  ![DMS UI](/img/dms-ui.jpg)
 But, before we deep dive into building the Document Management System(DMS), lets understand what Microservice is, and why it is good and how do we build one.



**Microservices** is an architectural style/approach followed while building a complex software applications. In Microservices-based architecture, instead of **building**, **packaging** and **deploying** a complex enterprise application as a single deployable artifact(**\*.war**, **\*.ear**, ...etc), we decompose(break down) the complex application into one or more smaller **independent** services and we **build**, **package**, **test** and **deploy** them independently without one knowing the existence of the other, during runtime these smaller services **collaborate/compose** together to make up the complex software application.

**So what are the advantages Microservices?** Well, Microservices architectural style offers a lot of advantage over the monolithic architecture(_where the complex enterprise application is built, packaged and deployed as single archive._). <br>
The followings are some the advantages of Microservices: 

1. _**Flexiblity**_: Microservices gives the flexibility to scale only those services where scale. Build, test, package and deploy each services independently and can use different frameworks(or even different languages to build them). Microservices gives us the flexibility to rollback only those features that have failed, in monolithic applications we would have to rollback the entire application even though the failure is in a single feature.  

2. _**Do it well(lesser chances for errors)**_: A Microservice has a small(But, _**Small is Beautiful**_, right?) **scope/feature** as such there are lesser chances that something can go wrong, because smaller means less complex and less complex means easy to understand, isnt't it?. But, hey! anything can go wrong in this world... but you get my point here.<br>
Note that when we say small, it is not perfectly perfect to say that the codebase is also smaller.
3. **Reusability**: Since each components are independent and focused on implementing a single feature this same feature can be used in other applications.

4. **Good For Agile Development**: Imagine you have 25 developers all working on an enterprise application, imagine how noisy the daily stand up would be( where each developers supposed to give their status: what did you do yesterday?,  What will you be working on today? and do you have any impediments? ), the collaboration among all these 25 developers who have been very difficult. There should be no more 4 to 5 people working really closely in day-to-day basis. In Microservices-based architecture you break the complex application into multiple smaller services  and each team would just focus on building, testing deploying each services independently. Each team will have agreements(a well defined contracts depicting how to consume each service and what output each service give back..etc.) The contracts/agreements are usually documented using frameworks like Swagger. 

I hope you have learned something new! <button name="button" link="projects" class="button">Now Let's build our DMS using Microservices</button>

