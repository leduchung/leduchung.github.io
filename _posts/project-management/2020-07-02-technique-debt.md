---
title: "The quadrant of development"
categories:
 - project management
tags:
 - architecture
last_modified_at: 2020-07-02
---

What forms the value of an application? Let us talk about kinds of value.


We will discuss the quadrant below as the picture says itself

<img style="float: right;" width="400" src="/images/technical-debt.png">

# Feature, the visible positive value

Features are usually created based on the problem and user requirements. From a fundamental problem that the system wants to solve, more supporting features can be developed to gain more values, it is clear.

What makes good features, means more visible positive value?

- Very clear requirements - The team who builds the system must know the domain, at least to the level that they can handle the problem and transfer the problem into computer language.
- Agile - For software and small development team, agile methodology is crucial. Software engineering is much different from other domains.
- Technologies - Due to the rapid changes in IT, I do not doubt the statement "update yourself or you are out". Good features always come with the technologies you choose.

Are there bad features? Yes, there are, when a feature does not fit with user needs. So, understand the problem deeply is the key to produce useful features.

# Bug, the visible negative value

We all hate bugs. But we constantly create bugs along with features. We will lose users because of bugs despite how amazing our features are. A bug is like a fly that gets into your tasty drink. If you still leave the fly in your glass, will you continue to drink?

How to prevent bugs?

- Automation tests - Test is the most effective way of reducing the number of bugs. The coverage rate should be 100%, meaning all lines should be tests. Sometimes the testing tool cannot detect the correct coverage, but intentionally, developers should test everything they write.
- More users, more feedbacks - A bug sometimes only appear in a certain circumstance. Users' feedbacks are a very powerful method to improve the system. However, users' complaints must be a reliable response from the developers and good planning to fix bugs.

# Architecture - the invisible positive value

Architecture is invisible, so users cannot see it and even developers cannot see it. However, it enables an easy and effective way to manage the application lifecycle. We can name a few non-functional requirements of the code-base which can only be achieved by good architecture, like extensibility, maintainability, collaboration... or at the runtime like security, high availability.

How to create good architecture?

- Design patterns - Just follow best practices from great developers in history. These patterns can serve almost the purpose of an application.
- Microservices - Divide to conquer is the basic technique when designing a system. We are human, we can deal with a small problem easily. If you have a very big system, just think about how to divide it in various dimensions.

# Technical debt - the invisible negative value

Technical debt is the hidden bugs that do not show its damage at the time of creation. But longer the invisible bug will affect the system in a certain way. The longer the invisible bug staying there, the more dependency it collects, the harder to remove it.

How to reduce technical debt?

- Remove code smell - There are a lot of symptoms showing that you are creating troubles for yourself, called code smells. Using a tool to detect it. 
- Continuous refactoring - Whenever you pass by the code, try to improve it a bit. The code you left behind is always better than the code when you touch it. However, developers are hesitant to refactor because they are afraid of breaking it. To overcome fear, and automation test is the key. Again, we see testing is crucial to remove both visible and invisible values from the system.

