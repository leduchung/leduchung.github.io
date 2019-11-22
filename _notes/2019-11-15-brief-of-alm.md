---
title: "Beginning Application Lifecycle Management - the notes"
categories:
 - devops
tags:
 - ALM, book
last_modified_at: 2019-11-15
---

I take note the points in the book "Beginning Application Lifecycle Management" by Joachim Rossberg. Just a note for me.

# Chapter 1 - Why application Lifecycle Management Matters

 - The organization must be responding to the changes in the modern world
 - Business is not only the commercial part of the company but all the functions
 - Three cornerstones of business: process, business rules, and information
 - Business software is for turning business needs and opportunities into business value
 - Problems we face in today's business environment
    - Global environment: both opportunities and challenges
    - Business must become more agile
    - Communication becomes increasingly complex
 - Project health today - 3 criteria to success (but we need to be skeptical due to the rapid change):
    - Project delivered on time
    - Project delivered on budget
    - Project goals met
 - Factor influencing projects and their success
    - The gap between business and IT (security/availability/scalability v.s business processes)
    - The development process: must be simple and transparent under the tools, so developers can focus on the work but still follow the processes. Nowadays, processes must be flexible too
    - Geographic spread
    - Synchronization of tools
    - Resource management
    - Project size
 - Project success: Research says about ten reasons:
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

# Chapter 2 - Introduce to ALM

 - The ALM includes three parts: Porfolio rationalization, Software development lifecycle, and Operations. All combine into a unified view.
 - The three pillars of traditional ALM: Traceability, Process Automation, Visibility
 - ALM v1 and ALM v2: common functions are built in a common framework and enable integrating various extra functions
 - The change: from the requirement to backlog-driven work
 - Future ALM: Traditional (Traceability, Automation, Reporting) + Work planning + Collaborator
 - DevOps: bring Dev and Ops closer. Key concepts: Continuous development, continuous integration, continuous operations
 - DevOps purpose: optimize the time from the application development until it's running stably in the production

# Chapter 3 - Development processes and frameworks

 - Development process models
    - waterfall: top-down, one step must go after each other
    - spiral: create one prototype and improve it over time
    - RUP - rational unified process: adaptive, balance, collaborate, elevate abstraction, focus on quality --> too much to choose from, to extendable to adapt
    - Agile: highest priority is customer satisfaction
    - Complexity in projects: developers, requirements, technology (infrastructure) --> scrum try to implement "Empirical Process Control"
    - Roles in scrum:
      - The product owner: funding and deliver a product or system to give the best Return on Investment (ROI) --> inspect and prioritize the backlog
      - The team: development
      - The scrum master: scrum process
    - Kanban: can be integrated into the existing process
    - Recommendation: Agile method. Scrum for development and Kanban for operations

# Chapter 4 - Scrum and agile concept
  - User story, requirements and estimations, during sprint
  - How agile maps to ALM

# Chapter 5 - ALM Assessments

 - One should use tool to assess the ALM, e.g. to access the maturity of a service
 - Example: is the organization have a good code analysis
 - For a tool or process, you can assess in 4 level: Basic, Standardized, Rationalized/Advanced, Dynamic

# Chapter 6 - Visibility and Traceability

 - In Agile, Continuous Integration can increase the Visibility
 - Rules for CI
   - Check in often
   - Don't check in broken code
   - Fix broken code immediately
   - Write unit tests
   - All tests and inspections must pass
   - Run private build
   - Avoid getting broken code: reverted to the worked version
 - Components of CI:
   - Build automation: CI builds (lightweight, incremental) private build, nightly builds (complete build with exhaustive testing), release builds (complete with release notes)

# Chapter 7 - automation of processes

# Chapter 8 - Work planning

 - Task management must be integrated with other systems like requirement management, test management, bug tracking

# Chapter 9 - Collaboraton

 - Collaboration includes: communication, sharing information
 - DevOps covers: development, operations and QA
   - DevOps has no special method or process, but focus on 3 key concepts: continuous development, continuous integration, continuous operations

# Chapter 10 - Metric in ALM

 - Agile: Backlog, Burndown, Velocity, Release burndown, remaining work, unplanned work
 - Architecture, Analysis and Design: Lines of code, Class coupling, Depth of inheritance, Cyclomatic complexity and Maintainability index.
   - Some ALM tool can give: circular references, hubs, and unreferenced nodes
 - Developer practices: code coverage, code metric (similar to the above list), compiler warning, and code-analysis warning
 - Testing: Number of bugs per state, number of bugs sent back from testers for more information (reactivated bugs)
 - Release management: number of software defects in production, percentage of successful software upgrades, number of untested releases, number of urgent releases, average costs of releases

# Chapter 11 - Introduce to ALM platforms