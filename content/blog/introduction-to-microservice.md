+++
author = "Ahmedin Hassen"
categories = ["Microservice"]
tags = ["Java Tutorial", "MicroService", "Software", "Architectural Style", "Cloud native"]
date = "2018-12-09"
description = "Full Document management application build using microservice architectural style."
featured = "pic03.jpg"
featuredalt = "Pic 3"
featuredpath = "date"
linktitle = ""
title = "Inroduction to Microservices"
type = "post"

+++

## Introduction Microservice. 

In this tutorial I will show you how to create MicroServices using Spring Boot Framework and the best way to learn microservices is creating them, for that we are going to build a simple Document Management System using Microservice architecture. The Document Management System will enable us to upload a document(*.pdf, *.doc, *.txt... etc, even *.zip), search  document(search by content), update a document and delete a document(s).  This is what the UI will look like at the end ##insertScreenShot##  But, before we deep dive into building the Document Management System(DMS), lets understand what Microservice is, and why it is good and how do we build one.

Microservices is an architectural style/approach followed while building a complex software applications. In Microservices-based architecture, instead of building, packaging and deploying a complex enterpise applicatioin as a single deployable artifact, we decompose the complex application into one or more smaller independent services/components. We build, test and deploy each services independenently without one knowing the existance of the other. During runtime these smaller services colabrote/compose together inorder to make up the complex software application through someform of service communication medias(api call, json, jms etc...)


In monolethic architectural style you build, package and deploy your enterprise application a single deployable artifact(jar, war or ear). In monolethic base application code is packaged into a single archive and is  stored in a single directory.


So what is the benefits of decomposing  down the big complex software application? Well, the Microservices architectural style offers handful of benefits over the monolethic stlye where the complex enterprise application is build, packaged and deployed as single archive.

1. Flexiblity: Build, test, package and deploy each services independenctly and can use different frameworks(or even languages to build them)
2. Do it well: A single microservice a small feature or functionality. a single microservice has smaller scope but it does it very well.
3. Lesser chance of error: Since a single microservices is focusing on smaller scope and well defined one there is less chance that something can go wrong... (but, hey!, remember anything can go wrong in this world... but you get the point..)
4. Encourage upgrade: companys are afraid of touching there mission critical application once it is deployed in production because they are afraid of something can go wrong during deployemenemt or some tested code can be deployed... But, in microservices, CI/CD can be automated(with automation testing) and more than that a single services can be upgraded/deployed independently... while rest of the appliation still serving the customer...etc... it is okay if the amazon "Recommendation" service is not available as song as I can do everything else... in the monetich architecture the entire site will be down for the new deployment eventhoug hte change is in Remcommendation service... same thing goes for the Facebook 'notification' future...
5. Reusablity
6. ==Agile friendly==: imaging you have 25 developers all working on one enterpirse software system... imagine how difficult will be the stand up(while it supposed to be a 15 minutes meeting while everytone is anwsering the three questions..)... the meeting would have been turned into noices... there should be no more 4 to 5 people in a team in my opinion... So, in microservices you break the complex system into multiple smaller services and a team would just focus on building, testing deploying that single services without even worying who will be consuming the user of the service they are working...

So how do these team communicate together inorder to make sure that all these teams are working on a sigle goals... making complex sysetm up... where is the checkpoint... how does team 1 knows they building something what its consumer think they will get?
The answer is they will have an agreed upon sort of contract... a well defined documentation(swagger)... explaining this is what my service will give it to you if you communicate with it in this way(giving this and that informtion...)

I hope you have learned something new! <button name="button" onclick="/projects" class="button">Now Let's build our DMS using Microservices</button>

