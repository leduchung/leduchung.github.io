---
title: "Beginning Application Lifecycle Management - the notes"
categories:
 - devops
tags:
 - ALM
 - book
last_modified_at: 2019-11-15
---

It is my note about "Beginning Application Lifecycle Management", a book from Joachim Rossberg, published by www.apress.com.

As the title said, the book covers basic concepts of Application Lifecycle Management (ALM). The main flow of the book shows why ALM matters, and what technologies are available over the history of application development. Then the authors focus on the Agile methodologies and the many implementations around.

I feel the book is easy to read, even with beginners. For me, I could connect all pieces of knowledge into an overview of DevOps, in which area I have been working for a few years. The followings are some notes I think relevant to me.

# The why
The authors proved by explanations and examples that changing is a must for every organization in the modern business environment. The word "business" nowadays not only about the commercial part but include all functions across the organization. In that condition, organizations must ensure the following three pillars: process, business rules, and information. 

Then, the era of manual tasks has passed. Business software is built for turning business needs and opportunities into business value. The main challenge for this is the globalization of business that forces the development to become more agile. 

A project is defined to be successful must fulfill three conditions: 

 - The project delivered on time
 - The project delivered on budget
 - The project goal met

What hinders the project from success:

 - The gap between business and IT (security/availability/scalability v.s business processes)
 - The development process: must be simple and transparent under the tools, so developers can focus on the work but still follow the processes. Nowadays, processes must be flexible too
 - Geographic spread
 - Synchronization of tools
 - Resource management
 - Project size

Then researchers say about ten reasons that lead to a successful project:

 1. User involvement
 2. Executive management support
 3. Clear business objectives
 4. Optimizing scope
 5. Agile process
 6. Project manager expertise
 7. Financial management
 8. Skilled resources
 9. Formal methodology
 10. Standard tools and infrastructure

# The what

ALM includes three parts, in which later can be combined into a unified view:

 - Porfolio rationalization
 - Software development lifecycle
 - Operations

For non-function qualification, the three pillars of traditional ALM are Traceability, Process Automation, Visibility. The modern ALM adds two more pillars including Work planning and Collaborator. And due to the additional pillars, the application development must go agile and switch from requirment-driven work to backlog-driven work.

The DevOps concept appears when the need of connecting Development and Operations. With its technologies (Continuous development, continuous integration, continuous operations), DevOps purpose is to optimize the time from the application development until it's running stably in the production.

# The how

The later chapters of the book are all about concrete implementation focusing on Agile methodologies. The two favorite techniques are Scrum for Development and Kanban for Operations. Each pillar of modern ALM is explained very well in defails with examples of common framework from Microsoft, IBM, HP and Atlassian.

Chapter 10 is intesting where author show how we can evaluate our platform and services. For each topic, a list of sample metrics and their meanings clarifies of what we can focus on when setting up the development environment.

At the end, the book is a good starting point for us to further investigate on what we want to apply in our organizations. The concrete implementation, I believe, is much more complex than just a few chapters.


