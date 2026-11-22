 

University of Westminster Informatic Institute of Technology (IIT) 

Agile Team Project (ATP)

5COSC021C 

Module leader :  Mr. Banuka Athuraliya  
Group Number :  SE 21  
Group Supervisor: Bimali Wickremasinghe  

Group Members : 

| Student Name | UOW ID  | IIT ID | Group  |
| :---: | :---: | :---: | :---: |
| **Vyshali Panneer** | **w2120032** | **20232472** | **SE G03** |
| **Ravichandran Aarshidan** | **w2182343** | **20250378** | **SE G03** |
| **Mohammed Dawood Abdullah** | **w2182332** | **20241342** | **SE G02** |
| **Gnanarajah Vithushan** | **w2149550** | **20241920** | **SE G03** |
| **Mohamed Ilham Safry** | **w2151085** | **20233044** | **SE G04** |

1. # Declaration {#declaration}

We certify that this project report and its associated artefacts are our original work. It has not been submitted before, nor is it currently being submitted for any degree program. 

Full Name of Student: Vyshali Panneer   
IIT Id: 20232472  
UOW Id: w2120032

Full Name of Student:  Ravichandran Aarshidan  
IIT Id: 20250378  
UOW Id: w2182343

Full Name of Student: Mohammed Dawood Abdullah  
IIT Id: 20241342  
UOW Id : w2182332

Full Name of Student:Gnanarajah Vithushan  
IIT Id: 20241920  
UOW Id: w2149550

Full Name of Student: Abdul Lathif Mohamed Ilham Safry  
IIT Id: 20233044  
UOW Id: w2151085

# 

2. # Abstract {#abstract}

Every day, drivers in Sri Lanka find themselves stranded on the roadside with a vehicle that will not move. With more than 8.5 million registered vehicles in the country, breakdowns are common, yet there is no single place a driver can turn to for reliable help. Most people phone a mechanic they already know or search social media, and they are left worrying about who to trust, how to explain their location, whether the mechanic will have the right part, and how safe they will be while they wait, especially at night. 

FixMyRide is a mobile application designed to ease these worries. One app serves both drivers and mechanics. A driver reports a breakdown using their GPS location, sees verified mechanics nearby ranked by distance, rating and skill, and follows the mechanic's arrival live on a map. Four features set the app apart. Smart matching connects the driver with a mechanic suited to the problem. Inventory search shows which nearby mechanics carry the part that is needed. Safety share sends the trip and mechanic details to someone the driver trusts. A completion code and photo proof close each job clearly. 

This portfolio presents the client brief, the analysis of the problem, our Agile approach, the system requirements, the social, legal, ethical and professional issues, and the system design, including wireframes and a high-fidelity prototype. The team worked in Scrum sprints, with Sprint 0 and Sprint 1 completed in Semester 1\. Building and testing the application will follow in Semester 2\. 

3. #  Acknowledgement {#acknowledgement}

This project would not have been possible without the help of many people, and we would like to thank them here. 

First, we thank our Module Leader, Mr. Banuka Athuraliya, for the guidance and the opportunity to work on a real-world project through the Agile Team Project module. We are especially grateful to our supervisor, Bimali Wickremasinghe  , whose weekly feedback kept us on track and helped us improve our work at every stage. 

Our thanks go to the drivers and mechanics who answered our questions and shared their experiences, which shaped many of the decisions in FixMyRide. 

We are grateful to the Informatics Institute of Technology and the University of Westminster for the resources and learning environment they provided. We also thank our lecturers and friends for their advice and encouragement. 

Finally, we thank our families for their patience and support throughout this project. 

4. # Table of Contents {#table-of-contents}

[**I. Declaration	1**](#declaration)

[**II. Abstract	2**](#abstract)

[**III. Acknowledgement	3**](#acknowledgement)

[**IV. Table of Contents	4**](#table-of-contents)

[**V. List of Figures	8**](#list-of-figures)

[**VI. Abbreviation Table	9**](#abbreviation-table)

[**Chapter 1: Introduction	1**](#chapter-1:-introduction)

[1.1 Chapter Overview	1](#1.1-chapter-overview)

[1.2 Client and/or Project Brief	1](#1.2-client-and/or-project-brief)

[1.3 Problem Background	1](#1.3-problem-background)

[1.4 Problem Statement	2](#1.4-problem-statement)

[1.5 Proposed Solution	2](#1.5-proposed-solution)

[1.6 Aim	3](#1.6-aim)

[1.7 Project Scope	3](#1.7-project-scope)

[1.7.1 In-scope	3](#1.7.1-in-scope)

[1.7.2 Out-scope	4](#1.7.2-out-scope)

[1.8 Rich Picture Diagram	4](#1.8-rich-picture-diagram)

[1.9 Resource Requirements	5](#1.9-resource-requirements)

[1.9.1 Hardware Requirements	5](#1.9.1-hardware-requirements)

[1.9.2 Software Requirements	5](#1.9.2-software-requirements)

[1.9.3 Data Requirements (Optional)	6](#1.9.3-data-requirements-\(optional\))

[1.10 Business Model Canvas	6](#1.10-business-model-canvas)

[1.11 Chapter Summary	7](#1.11-chapter-summary)

[**Chapter 2: Existing Work	8**](#chapter-2:-existing-work)

[2.1 Chapter Overview	8](#2.1-chapter-overview)

[2.2 Competitor Analysis	8](#2.2-competitor-analysis)

[2.2.1 MyMech	8](#2.2.1-mymech)

[2.2.2 GarageGo	8](#2.2.2-garagego)

[2.2.3 Worky	9](#2.2.3-worky)

[2.2.4 Feature Comparison of Existing Applications with Fix My Ride	9](#2.2.4-feature-comparison-of-existing-applications-with-fix-my-ride)

[2.2.3 Research Gap and Project Opportunity	9](#2.2.3-research-gap-and-project-opportunity)

[2.3 Technology Selection and Implementation Approach	10](#2.3-technology-selection-and-implementation-approach)

[2.3.1 Technology Stack	10](#2.3.1-technology-stack)

[2.3.2 Implementation Approach	11](#2.3.2-implementation-approach)

[2.4 Chapter Summary	12](#2.4-chapter-summary)

[**Chapter 3: Agile Approach and Project Management	13**](#chapter-3:-agile-approach-and-project-management)

[3.1 Chapter Overview	13](#3.1-chapter-overview)

[3.2 Agile Framework Selection	13](#3.2-agile-framework-selection)

[3.3 System Analysis and Design Methodology	13](#3.3-system-analysis-and-design-methodology)

[3.3.1 Methodology Selection and Justification (OOADM / SSADM)	13](#3.3.1-methodology-selection-and-justification-\(ooadm-/-ssadm\))

[3.3.2 Application of the Selected Methodology	14](#3.3.2-application-of-the-selected-methodology)

[3.4 Team Roles and Responsibilities	16](#3.4-team-roles-and-responsibilities)

[Table 9: Team roles and responsibilities	16](#table-9:-team-roles-and-responsibilities)

[3.5 Sprint Structure and Agile Ceremonies	16](#3.5-sprint-structure-and-agile-ceremonies)

[3.5.1 Sprint Structure and Ceremonies	16](#3.5.1-sprint-structure-and-ceremonies)

[3.5.2 Definition of Ready and Definition of Done	16](#3.5.2-definition-of-ready-and-definition-of-done)

[3.5.3 Team Working Agreement	16](#3.5.3-team-working-agreement)

[3.6 Tools and Version Control Workflow	17](#3.6-tools-and-version-control-workflow)

[3.7 Communication Plan	17](#3.7-communication-plan)

[3.8 User Needs and Requirements Definition	18](#3.8-user-needs-and-requirements-definition)

[3.8.1 User Personas	18](#3.8.1-user-personas)

[3.8.2 User Stories	18](#3.8.2-user-stories)

[3.9 Product Backlog	18](#3.9-product-backlog)

[3.9.1 Backlog Creation and Prioritisation	19](#3.9.1-backlog-creation-and-prioritisation)

[3.9.2 Prioritised Product Backlog	19](#3.9.2-prioritised-product-backlog)

[3.9.3 Task Board Evidence	19](#3.9.3-task-board-evidence)

[3.10 Release Plan / Roadmap	19](#3.10-release-plan-/-roadmap)

[3.11 Risks and MitigationTable 14: Risk register	20](#3.11-risks-and-mitigationtable-14:-risk-register)

[3.12 Chapter Summary	20](#3.12-chapter-summary)

[**Chapter 4: System Requirements Specification (SRS)	21**](#chapter-4:-system-requirements-specification-\(srs\))

[4.1 Chapter Overview	21](#4.1-chapter-overview)

[4.2 Stakeholder Analysis	21](#4.2-stakeholder-analysis)

[4.2.1 Onion Model	22](#4.2.1-onion-model)

[4.2.2 Stakeholder Descriptions	22](#4.2.2-stakeholder-descriptions)

[4.3 Selection of Requirement Elicitation Techniques / Methods	24](#4.3-selection-of-requirement-elicitation-techniques-/-methods)

[4.4 Discussion / Analysis of Results	25](#4.4-discussion-/-analysis-of-results)

[4.5 Use Case Diagram	27](#4.5-use-case-diagram)

[4.6 Use Case Descriptions	28](#4.6-use-case-descriptions)

[4.7 Functional Requirements	42](#4.7-functional-requirements)

[Table 17: Functional requirements	42](#table-17:-functional-requirements)

[4.8 Non-Functional Requirements	43](#4.8-non-functional-requirements)

[Table 18: Non-functional requirements	43](#table-18:-non-functional-requirements)

[4.9 Assumptions and Clarifications	44](#4.9-assumptions-and-clarifications)

[Table 19: Assumptions and clarifications	44](#table-19:-assumptions-and-clarifications)

[4.10 Chapter Summary	46](#4.10-chapter-summary)

[**Chapter 5: Social, Legal, Ethical and Professional Issues	47**](#chapter-5:-social,-legal,-ethical-and-professional-issues)

[5.1 Chapter Overview	47](#5.1-chapter-overview)

[5.2 Ethical Clearance	47](#5.2-ethical-clearance)

[5.3 SLEP Issues and Mitigation	47](#5.3-slep-issues-and-mitigation)

[**5.3.1 Legal Issues	47**](#5.3.1-legal-issues)

[**5.3.2 Ethical issues	48**](#5.3.2-ethical-issues)

[**5.3.3  Security Issue	49**](#5.3.3-security-issue)

[**5.3.4 Equality, Diversity and Inclusion	50**](#5.3.4-equality,-diversity-and-inclusion)

[**5.3.5 Sustainability	51**](#5.3.5-sustainability)

[**5.3.6 Professional Issues	51**](#5.3.6-professional-issues)

[5.4 Chapter Summary	51](#5.4-chapter-summary)

[**Chapter 6: System Architecture and Design	52**](#chapter-6:-system-architecture-and-design)

[6.1 Chapter Overview	52](#6.1-chapter-overview)

[6.2 System Architecture Design	52](#6.2-system-architecture-design)

[6.3 System Design	53](#6.3-system-design)

[6.3.1 Class Diagram / Data Flow Diagram (DFD)	53](#6.3.1-class-diagram-/-data-flow-diagram-\(dfd\))

[6.3.2 Sequence Diagram	53](#6.3.2-sequence-diagram)

[6.3.3 Activity Diagram	53](#6.3.3-activity-diagram)

[6.4 User-Centred Design and UI/UX	53](#6.4-user-centred-design-and-ui/ux)

[6.4.1 Wireframes	53](#6.4.1-wireframes)

[6.4.2 UI/UX (Figma)	53](#6.4.2-ui/ux-\(figma\))

[6.5 Design Principles and Sustainability	53](#6.5-design-principles-and-sustainability)

[6.6 Chapter Summary	54](#6.6-chapter-summary)

[**Chapter 7: Sprint Records	55**](#chapter-7:-sprint-records)

[7.1 Chapter Overview	55](#7.1-chapter-overview)

[7.2 Sprint 0 – Inception and Set-up	56](#7.2-sprint-0-–-inception-and-set-up)

[7.2.1 Sprint Goal and Dates	56](#7.2.1-sprint-goal-and-dates)

[7.2.2 Sprint Planning and Sprint Backlog	56](#7.2.2-sprint-planning-and-sprint-backlog)

[7.2.3 Stand-up and Progress Summary	56](#7.2.3-stand-up-and-progress-summary)

[7.2.4 Increment Delivered	57](#7.2.4-increment-delivered)

[7.2.5 Sprint Review and Feedback	57](#7.2.5-sprint-review-and-feedback)

[7.2.6 Sprint Retrospective	57](#7.2.6-sprint-retrospective)

[7.3 Sprint 1 – Requirements and Design Increment	57](#7.3-sprint-1-–-requirements-and-design-increment)

[7.3.1 Sprint Goal and Dates	57](#7.3.1-sprint-goal-and-dates)

[7.3.2 Sprint Planning and Sprint Backlog	57](#7.3.2-sprint-planning-and-sprint-backlog)

[7.3.3 Stand-up and Progress Summary	58](#7.3.3-stand-up-and-progress-summary)

[7.3.4 Increment Delivered	58](#7.3.4-increment-delivered)

[7.3.5 Sprint Review and Feedback	58](#7.3.5-sprint-review-and-feedback)

[7.3.6 Sprint Retrospective	58](#7.3.6-sprint-retrospective)

[7.4 Sprint 2	58](#7.4-sprint-2)

[7.4.1 Sprint Goal and Dates	58](#7.4.1-sprint-goal-and-dates)

[7.4.2 Sprint Planning and Sprint Backlog	59](#7.4.2-sprint-planning-and-sprint-backlog)

[7.4.3 Stand-up and Progress Summary	59](#7.4.3-stand-up-and-progress-summary)

[7.4.4 Increment Delivered	59](#7.4.4-increment-delivered)

[7.4.5 Sprint Review and Feedback	59](#7.4.5-sprint-review-and-feedback)

[7.4.6 Sprint Retrospective	59](#7.4.6-sprint-retrospective)

[7.5 Sprint 3	59](#7.5-sprint-3)

[7.5.1 Sprint Goal and Dates	59](#7.5.1-sprint-goal-and-dates)

[7.5.2 Sprint Planning and Sprint Backlog	59](#7.5.2-sprint-planning-and-sprint-backlog)

[7.5.3 Stand-up and Progress Summary	60](#7.5.3-stand-up-and-progress-summary)

[7.5.4 Increment Delivered	60](#7.5.4-increment-delivered)

[7.5.5 Sprint Review and Feedback	60](#7.5.5-sprint-review-and-feedback)

[7.5.6 Sprint Retrospective	60](#7.5.6-sprint-retrospective)

[7.6 Sprint 4	60](#7.6-sprint-4)

[7.6.1 Sprint Goal and Dates	60](#7.6.1-sprint-goal-and-dates)

[7.6.2 Sprint Planning and Sprint Backlog	60](#7.6.2-sprint-planning-and-sprint-backlog)

[7.6.3 Stand-up and Progress Summary	60](#7.6.3-stand-up-and-progress-summary)

[7.6.4 Increment Delivered	60](#7.6.4-increment-delivered)

[7.6.5 Sprint Review and Feedback	61](#7.6.5-sprint-review-and-feedback)

[7.6.6 Sprint Retrospective	61](#7.6.6-sprint-retrospective)

[7.7 Test Strategy	61](#7.7-test-strategy)

[7.7.1 Testing Approach	61](#7.7.1-testing-approach)

[7.7.2 Test Case Template	61](#7.7.2-test-case-template)

[7.7.3 Coding Standards and Traceability	61](#7.7.3-coding-standards-and-traceability)

[7.8 Chapter Summary	61](#7.8-chapter-summary)

[**Chapter 8: Individual Contributions	62**](#chapter-8:-individual-contributions)

[8.1 Chapter Overview	62](#8.1-chapter-overview)

[8.2 Verification of Individual Contribution	62](#8.2-verification-of-individual-contribution)

[8.3 Contribution Summary by Member	62](#8.3-contribution-summary-by-member)

[8.4 Chapter Summary	62](#8.4-chapter-summary)

[**References	63**](#references)

[**Appendices	64**](#heading=)

5. # List of Figures {#list-of-figures}

   [Figure 1: Business Model Canvas	6](#figure-1:-business-model-canvas)

   

6. # Abbreviation Table {#abbreviation-table}

| Abbreviation | Full form |
| :---: | :---: |
| API | Application Programming Interface |
| ATP | Agile Team Project |
| DMT | Department of Motor Traffic |
| GB | Gigabyte |
| GPS | Global Positioning System |
| ID | Identification |
| RAM | Random Access Memory |
| SMS | Short Message Service |
| SSD | Solid State Drive |
| UML | Unified Modeling Language |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |

# **Chapter 1: Introduction** {#chapter-1:-introduction}

## **1.1 Chapter Overview** {#1.1-chapter-overview}

This chapter introduces FixMyRide, a single mobile application that connects drivers whose vehicles have broken down with nearby, verified mechanics. It presents the client brief, explains the problem with supporting evidence and example scenarios, and states the problem in one sentence. It then describes the proposed solution and its aim, sets out what the team will and will not build, and closes with a rich picture, the resources needed for the minimum viable product and a business model canvas.

## 

## **1.2 Client and/or Project Brief** {#1.2-client-and/or-project-brief}

| *Summarise the project brief set by the external or simulated client. Identify the client, their organisation and their needs, and how the team communicates with them (e.g. client meetings, emails, feedback sessions). Include evidence of client communication in the appendix (Appendix C).*  |
| :---- |

## 

## **1.3 Problem Background** {#1.3-problem-background}

Sri Lanka has a lot of vehicles, and the number keeps growing. By May 2025, the Department of Motor Traffic had recorded 8,528,002 registered vehicles. This includes 4,981,211 motorcycles, 1,186,220 three-wheelers and 912,871 cars (Daily FT, 2025). New vehicles are still being added. For example, more than 223,000 new motorcycles were registered between January and early December 2025 (Ada Derana, 2025). With so many vehicles on the road, it is fair to expect many drivers to face a breakdown, such as a flat tyre, a dead battery or an engine problem.

When a vehicle breaks down, there is no single place a driver can trust for help. Most people call a mechanic they already know, ask someone nearby, or search social media. This leads to a few problems:

* **Help is slow and uncertain.** The driver does not know which mechanics are nearby, free or honest.  
* **The price is unclear.** The price is often discussed on the roadside, when the driver is already stuck and cannot bargain much.  
* **Location is hard to explain.** It takes time to describe where you are on a road you do not know.  
* **The part may be missing.** A mechanic may arrive without the part and have to go back, so the wait becomes twice as long.  
* **Safety is a worry.** Waiting alone, especially at night, and trusting a stranger with your vehicle is risky. This is even harder for women, older drivers and people travelling alone.

**The following scenarios illustrate the problem.**

**Scenario 1 – A puncture at night.** A woman is driving between two towns late in the evening. Her tyre goes flat on a quiet road. She does not know any mechanic in the area and cannot explain exactly where she is. She is also not sure if the price she is told on the phone is fair. She waits alone, and her family cannot see what is happening.

**Scenario 2 – A dead motorcycle battery.** A man's motorcycle will not start in a town he does not know. He calls two garages, but neither can say if they have the right battery. A mechanic comes, finds he does not have one, and has to go back to get it.

**Scenario 3 – A three-wheeler driver losing income.** A three-wheeler driver's vehicle breaks down. Every hour it stays off the road costs him money. He needs a mechanic who can reach him fast and tell him the price before starting work.

**What makes FixMyRide different?** FixMyRide tackles the three biggest worries: price, parts and safety. The driver approves the price before the mechanic is sent. The driver can search for mechanics who really have the part. The driver can share the trip and the mechanic's details with someone they trust. At the end, a completion code and photos show that the job was done.

## 

## **1.4 Problem Statement** {#1.4-problem-statement}

Drivers in Sri Lanka  who break down have no reliable,clear and safe way to find a nearby mechanic,agree on a fair price and be sure the right parts will arrive 

## 

## **1.5 Proposed Solution** {#1.5-proposed-solution}

FixMyRide is one mobile app with two main roles: Driver and Mechanic. It works a bit like a ride-hailing app, but for roadside repairs.

The driver reports a breakdown by sharing their GPS location, vehicle details and the type of problem. The app shows mechanics nearby on a map, ranked by distance, rating and skill (for example tyres, batteries, engines or towing). The driver can also search for mechanics who have the part they need. The mechanic sends a price based on a fixed price list, and the driver approves it before the mechanic is sent. Then the driver can watch the mechanic's live location and arrival time, and call or chat with them.

For safety, the driver can send a trip link, the mechanic's name, photo and plate number to someone they trust. There is also an emergency button that calls 119 or 1990 and shares the driver's location. When the work is finished, the driver gives the mechanic a completion code, and photos from before and after are saved as proof. Both sides can then rate each other, and everyone can see their past requests. In the first version, payment is in cash after the job, at the price the driver approved.

## 

## **1.6 Aim** {#1.6-aim}

To build one easy-to-use mobile app that helps drivers in Sri Lanka find a verified mechanic nearby,agree on a fair price and feel safe during a breakdown.

In simple words, we want to remove the confusion and risk that drivers face. The mechanic, the price, the parts and the progress of the job should all be clear from the moment a request is made. For mechanics, we want to bring them regular jobs nearby and let them show they can be trusted through ratings and verification.

## 

## **1.7 Project Scope** {#1.7-project-scope}

This scope is for the first working version of the app (the minimum viable product). It can change as the sprints go on, and we will record any agreed changes in Chapter 7\.

## 

## **1.7.1 In-scope** {#1.7.1-in-scope}

**Driver features**

1. Registration and login  
2. Breakdown request with GPS location, vehicle details and problem type  
3. Nearby mechanics shown on a map with distance and rating  
4. Smart matching: mechanics ranked by distance, rating and skill  
5. Inventory search: find nearby mechanics who have the needed part  
6. Price quote approval before the mechanic is dispatched  
7. Live mechanic location and estimated arrival time  
8. Call or chat with the mechanic  
9. Safety share: trip link, mechanic name, photo and plate number sent to a trusted contact  
10. Job completion code with before and after photos  
11. Ratings, reviews and request history  
12. Emergency button that dials 119 or 1990 and shares location

**Mechanic features**

1. Registration and login with details and ID upload  
2. Online or offline availability toggle  
3. Inventory management (parts, availability and prices)  
4. Receive job requests, accept or reject, and send a price quote  
5. Update job status (Accepted, On the way, Working, Completed)  
6. Navigation to the customer  
7. Enter the completion code and upload before and after photos  
8. View ratings and job history

**Other in-scope decisions**

* One application for all users, with role-based screens  
* Mechanic verification is recorded as a verified flag in the database for the demonstration  
* Payment is cash on completion, using the approved quote

## **1.7.2 Out-scope** {#1.7.2-out-scope}

* A separate admin portal and user management screens (future work)  
* IoT devices or vehicle sensors  
* Online payment gateways  
* AI-based fault diagnosis and voice assistant  
* Insurance claims  
* Community forum and rewards system  
* Offline SMS request mode  
* Ordering or delivery of spare parts


## **1.8 Rich Picture Diagram** {#1.8-rich-picture-diagram}

## **1.9 Resource Requirements** {#1.9-resource-requirements}

These are the resources needed to build the first working version. We explain the final technology choices in Chapter 2\.

## 

## **1.9.1 Hardware Requirements** {#1.9.1-hardware-requirements}

| Hardware | Purpose |
| ----- | ----- |
| Laptops for each team member (suggested minimum: 8 GB RAM, SSD) | Development, design and documentation |
| Android smartphones (and an iPhone if iOS testing is planned) | Testing GPS, calls, notifications and live tracking |
| Reliable internet connection | Cloud services, maps and team collaboration |

## 

## **1.9.2 Software Requirements** {#1.9.2-software-requirements}

| Software | Purpose |
| ----- | ----- |
| Mobile framework (for example Flutter, as proposed) | Building the single cross-platform app |
| Backend and database (for example Node.js with Firebase or MongoDB, as proposed) | Accounts, requests, inventory and job data |
| Map and location service (for example Google Maps Platform) | Map display, distance, routes and live tracking |
| Git and GitHub | Version control and code review |
| Task board (Jira, Trello or GitHub Projects) | Backlog and sprint management |
| Figma | Wireframes and high-fidelity prototype |
| Draw.io | UML, architecture and rich picture diagrams |
| Google Docs | Portfolio writing with version history |
| Canva | Presentation slides |

## 

## **1.9.3 Data Requirements (Optional)** {#1.9.3-data-requirements-(optional)}

Not needed. FixMyRide does not use machine learning, so we do not need training data. We will create sample data for mechanics, parts and prices for testing.

## 

## **1.10 Business Model Canvas** {#1.10-business-model-canvas}

####                           ***Figure** 1**:** Business Model Canvas*  {#figure-1:-business-model-canvas}

## 

## **1.11 Chapter Summary**  {#1.11-chapter-summary}

This chapter explained the problem drivers face when their vehicle breaks down in a country with more than 8.5 million registered vehicles. Finding a mechanic, agreeing on a price and staying safe are all hard today. We introduced FixMyRide, one app that connects drivers with verified mechanics nearby. It has four special features: price quote approval, inventory search, safety share and a job completion code. We also set the scope, rich picture, resources and business model for the first version. The next chapter looks at existing solutions and chooses the technologies we will use.

# **Chapter 2: Existing Work** {#chapter-2:-existing-work}

## **2.1 Chapter Overview** {#2.1-chapter-overview}

This chapter explores existing applications and platforms that provide services similar to our proposed system. It focuses on how these platforms correct customers with service providers, allow business to advertise their services, and help users find products and services based on their needs and location

The chapter reviews existing platforms related to mechanic services, hardware shops, online marketplaces, and location based services. By looking at their features and how they work, we can understand the benefits they offer and identify areas that could be improved. This will help us  understand what users expect from this type of platform and how our proposed application can provide a useful solution.

In addition, this chapter discusses the main technologies that could support our application, such as inventory searching, GPS and real time location tracking, push notifications, emergency SOS, and chatbot assistance. These technologies will help bring mechanics, hardware shop owners, and the general public together through one platform.

## **2.2 Competitor Analysis** {#2.2-competitor-analysis}

Competitor analysis helps us understand how existing platforms provide services similar to our proposed application. By studying these platforms, we can identify their main features, strengths, and areas where our system could offer additional value.

For FixMyRide, Three existing platforms have been selected: MyMech, GarageGo and Worky. because they provide services related to finding mechanics, requesting services, and connecting customers with service providers. 

## **2.2.1 MyMech** {#2.2.1-mymech}

MyMech is a srilankan platform that connects vehicle owners with mechanics and garages. It provides services such as vehicle repairs, maintenance, inspections, breakdown assistance, service bookings and spare parts searching.

Main features: Mechanic discovery, vehicle maintenance, breakdown assistance, service bookings and spare parts searching.

Relevance to FixMyRide: Provides useful ideas for mechanic registration, service listings, nearby mechanic searching and inventory management.

## **2.2.2 GarageGo** {#2.2.2-garagego}

GarageGo is a vehicle assistance platform that allows customers to request maintenance and repair services at their location. It connects customers with nearby technicians and provides service requests, technician offers, live location tracking and in app communication.

Main features: On demand mechanic services, nearby technician discovery, service requests, live tracking and notifications.

Strengths: Makes it convenient for customers to find technicians and follow their location while waiting for a service.

Relevance to fixMyRide: Provides useful ideas for nearby mechanic searching, service requests, GPS and real time tracking.

## **2.2.3 Worky** {#2.2.3-worky}

Worky is a Srilankan service platform that connects people who need services with individuals who can provide them. Users can publish their requirements, discover available service providers, and connect with workers for different types of jobs, including home repairs and professional services.

Main features: Service listings, job requests, service provider discovery, location based services and direct communication.

Strengths: Supports different services categories and gives individuals an opportunity to offer their skills and connect with potential customers.

Relevance to FixMyRide: Provides useful ideas for public user requests, mechanic and hardware service listings and connecting customers with service providers.

## **2.2.4 Feature Comparison of Existing Applications with Fix My Ride** {#2.2.4-feature-comparison-of-existing-applications-with-fix-my-ride}

| Features | MyMech | GarageGo | Worky | FixMyRide |
| :---- | :---- | :---- | :---- | :---- |
| Real time GPS | **✗**  | **✓**  | **✗** (limited) | **✓**  |
| Real time tracking | **✗**  | **✓**  | **✗** (limited) | **✓**  |
| Push Notifications | **✗**  | **✓**  | **✓**  | **✓**  |
| Emergency sos | **✗**  | **✗**  | **✗**  | **✓**  |
| Chatbot | **✗**  | **✗**  | **✗**  | **✓**  |
| Inventory Searching | **✗** (limited) | **✗**  | **✗**  | **✓**  |
| Nearby service providers | **✓**  | **✓**  | **✓**  | **✓**  |

## **2.2.3 Research Gap and Project Opportunity** {#2.2.3-research-gap-and-project-opportunity}

Existing platforms provide useful services, but most focus on specific areas, such as finding mechanics or connecting customers with service providers. Users may still need to use different platforms to find mechanics, request services and search for available products.

FixMyRide aims to address this gap by bringing mechanics, hardware shop owners and the general public together in one platform. Mechanics and shop owners can list their services and inventory, while the public can report  problems, request services, find nearby mechanics and search for products.

The application will also include real time GPS, live tracking, Push notifications, emergency SOS, and chatbot assistance. These features aim to make finding vehicle related services and products easier and more convenient for users.

## **2.3 Technology Selection and Implementation Approach** {#2.3-technology-selection-and-implementation-approach}

Developing FixMyRide requires suitable technologies to support its main features, such as user accounts, service listings, inventory searching, GPS tracking, push notifications, and chatbot assistance. The selected technologies should be reliable, secure , user friendly and flexible enough to support future improvements.

The application will use a client server approach. The frontend will provide an easy to use interface for mechanics, hardware shop owners and the general public. The backend will manage user requests and application functions while the database will store user details, service information and product inventories.

GPS and location based technologies will help users find nearby mechanics and track service requests. Push notifications will keep users updated, while chatbot assistance will help them find relevant information and services.

The project will follow an incremental development approach, where features are developed and tested in smaller stages. This will help the team identify issues early, improve the application, and make changes based on testing and user feedback.

## **2.3.1 Technology Stack** {#2.3.1-technology-stack}

FixMyRide will use a combination of technologies to develop the mobile application, manage data, provide location based services, and support communication between users. The selected technologies are based on the project’s requirements and ease of development.

Flutter will be used to develop the mobile application, allowing the team to build a single app for different user roles. Spring Boot will handle the backend logic, including service requests, mechanic details, inventory management, and other application functions. MongoDB will be used to store user information, service details, product inventories, and ratings.

Firebase services will support authentication, notifications and file storage. Google Maps platform will be used for location based features, such as finding nearby mechanics and tracking service requests. Git and GitHub will support version control and teamwork, while Figma will be used to design the application’s interfaces and prototypes.

| Component | Technology | Why we use it |
| :---- | :---- | :---- |
| Frontend | Flutter | Develops one mobile application with role based screens for mechanics, hardware shop owners and the general public. |
| Backend  | Spring Boot / Firebase | Spring Boot handles application logic, requests, and services, while Firebase supports related cloud |
| Database  | MongoDB | Stores user details, service requests, mechanic information, inventory and ratings. |
| Authentication | Firebase Authentication | Provides secure login for different user types. |
| Maps and navigation | Google Maps Platform(Maps SDK, Directions, Distance Matrix) | Helps users find nearby mechanics, view routes, and check estimated arrival times. |
| Live location tracking | Firestore real time updates with Google Maps | Displays the mechanic’s live location on the user’s map. |
| Photo and ID storage | Firestore for chat; phone dialer for calls | Supports in app communication and direct phone calls |
| Safety share | Phone’s share option (SMS or WhatsApp) | Allows users to share service details and location with trusted contacts. |
| Notifications | Firebase Hosting / Google Cloud  | Sends alerts about new requests, service updates, and status changes. |
| Hosting | Firebase Hosting / Google Cloud | Hosts the backend related services and landing page. |
| Version control and board | Git and GitHub; Jira, Trello or GitHub Projects | Support teamwork, code reviews, and task tracking. |
| Design | Figma | Helps create wireframes and high fidelity prototypes. |

## **2.3.2 Implementation Approach** {#2.3.2-implementation-approach}

FixMyRide will be developed using an incremental approach, where the application is built in smaller stages rather than developing everything at once. Each stage will be implemented and tested before moving to the next, helping the team identify problems early and make improvements.

| Development stage | Implementation |
| :---- | :---- |
| User Management | Develop registration, login, and role based access for mechanics, hardware shop owners, and the public. |
| Service Listings | Allow mechanics and shop owners to publish their services and available inventory. |
| Service Requests | Allow users to report problems, request services and connect with relevant providers. |
| Inventory Search | Enable users to search for products and check available inventory. |
| Location Features | Implement GPS, nearby mechanic discovery, and real time tracking. |
| Communication | Add chat, notifications, chatbot assistance and emergency SOS features. |
| Testing and Improvement | Test the application, identify errors and improve features based on result and feedback |

## **2.4 Chapter Summary** {#2.4-chapter-summary}

This chapter reviewed existing platforms related to mechanic services and services and service provider connections, focusing on MyMech, GarageGo and Worky. The competitor analysis helped identify their main features and areas where FixMyRide could provide additional value. The research gap highlighted the need for a single platform connecting mechanics, hardware shop owners and the general public while providing service requests, inventory searching, and location based  features.  
The chapter also discussed the technologies selected for FixMyRide and the proposed implementation approach. These technologies and development stages provide a foundation for building the application and supporting its main features.

# Chapter 3: Agile Approach and Project Management {#chapter-3:-agile-approach-and-project-management}

## **3.1 Chapter Overview** {#3.1-chapter-overview}

| *Chapter talks about the way our project was implemented and blue-printed out using diagrams and how while framework made the project cohesive and flexible among our members.*  |
| :---- |

## **3.2 Agile Framework Selection** {#3.2-agile-framework-selection}

Scrum methodology was decided to be used, as split work load provided more flexibility to our group members by allowing them to work more freely during each sprint. Reviews and critiques allow members to see potential flaws and improve their work	

## **3.3 System Analysis and Design Methodology** {#3.3-system-analysis-and-design-methodology}

### **3.3.1 Methodology Selection and Justification (OOADM / SSADM)** {#3.3.1-methodology-selection-and-justification-(ooadm-/-ssadm)}

FixMyRide uses OOADM methodology and real world entities whose attributes are mapped directly to object oriented classes, rather than static data flows. 

|  | OOADM | SSADM |
| :---- | :---- | :---- |
| Core Architecture perspective | This project is driven around model drivers, mechanics, hardware supply stores, which are real world objects. This allows the system to be modelled as interactable objects. | The real world objects such as mechanics, drivers and hardware stores are stored as static database records rather than interactive objects. |
| Documentation perspective | Flexible and not heavy documentation while also being directly cohesive to the development path. | Extensive Documentation at each sprint or record. |
| Industry perspective | Object oriented pathways are critical and demanding in the modern software development world. | Although SSADMM is commercially used, it is rather not flexible and can be used for important tasks like the local government.  |
| Handling / Real time system usage | Objects are handled in order and algorithmically and assigned tasks and communicate with other objects. (live tracking and algorithmic calculations used ) | Real-time tasks handling aren’t suited for SSADM, since it mainly focuses on static data stor age. |

**Justification** \- fixMyRide project crucially revolves around taking real-life entities as object classes. Features such as real-time chats and tracking and allowing users to compliment each other are based on OOADM methodology.

### **3.3.2 Application of the Selected Methodology** {#3.3.2-application-of-the-selected-methodology}

This section explains how our team applies OOADM during system analysis and design and outlines the modelling techniques and UML diagrams we used to plan our application.  
   
OOADM is an approach that views a system as a set of cooperating objects and builds models of those objects step by step from requirements to implementation. FixMyRide is built around real-world entities such as drivers, mechanics, vehicle hardware stores, spare parts, and live GPS sessions OOADM gives us a straightforward way to turn user requirements into working software.

Pairing OOADM with our Scrum workflow keeps the process flexible. Instead of trying to design every detail upfront in one rigid phase, we pull tasks from our board continuously, model and refine them during the Coursework (members are assigned to their own tasks and help people) and build them thoroughly in Semester 2\. Core features like nearby service providing, live location sharing, and hardware inventory lookup can therefore be designed and tested as separate modules. 

Analysis, design, implementation and testing are crucial during each sprint or task log. Questionnaires and articles about mechanics’, vehicle owners’ and personal experiences are analysed. Analysis such as this is broken down into the objects needed.

In the design stage, we add technical details to initial models. The team decides how the Flutter mobile app will pull live coordinates using the Google Maps API or how the Spring Boot backend will use algorithms to handle proximity searches and spare-parts queries, and how Firebase services (Cloud Firestore, Realtime Database, and chat/call modules) will sync live GPS pins and direct communication. We capture the exact order of messages between these components in Sequence Diagrams, and map out step-by-step user decisions in Activity Diagrams. 

During implementation and testing, the design models are turned into working features across the Flutter frontend, Spring Boot backend, and Firebase services. Our code is hosted on GitHub using feature branches so different members can work on separate parts such as the live mechanic map and the hardware store inventory search in parallel during a sprint. Before any story is marked complete, the feature goes through unit tests in Spring Boot, UI and integration checks in Flutter, and real-world GPS testing on mobile phones so it meets our Definition of Done ahead of the Sprint Review.

At the end of each sprint, we demonstrate our progress and prototypes during the Sprint Review with our supervisor and gather feedback. When feedback leads to changes such as adjusting how drivers filter spare parts or rate mechanics we refine the Product Backlog and bring those updates into the next sprint. Because OOADM keeps data and logic grouped inside separate classes, updating one feature rarely requires rewriting unrelated parts of the app.	

**Modeling techniques**

* Use-case modeling used, shows the requirements of a  system from different users / actor perspectives.   
* Interaction modelling to track message and data sequence classes, APIs, cloud and servers over time.  
* Activity modelling for showing the work flow of the application’s system.  
* Data flow modeling used to map out information flow in a system from start to finish.

**Use Case Diagram**: The detailed Use Case diagram clarifies what FixMyRide must do from the objects of its three user groups: Drivers, Mechanics, Hardware. For a stranded driver, it covers nearby-service providers,real time tracking, sharing gps and hardware stock availability. For service providers, it covers toggling availability, live tracking, sharing spare parts and updating inventory. Keeping every requirement in chapter 4 tied directly to a real user goal. 

**Class Diagram:** Class diagram acts as a structure blueprint for both our spring boot backend classes and cloudbase firestore database collections. Common user details are placed in base User class, while mechanics and hardware store inherit from an abstract Service provider class. Since they share most classes like location, availability. It also shows how hardware stores links to inventory items for spare-parts searches, and how live tracking and shared gps and chat sessions handle live coordination between a driver and mechanic.

**Sequence Diagram:** shows how this application handles live roadside assistance connections across five different life lines: Driver (Flutter), Google maps API and sends a proximity request to spring boot, which queries cloudbase firestore and returns the nearest available mechanics. When the driver picks a mechanic and initiates contact, firebase’s realtime support syncs live gps movement between both phones while firebase  handles the in-app chat or voice call..

**Activity Diagram:** The activity Diagram goes through step by step flow of a user's experiences in the app. Being the user's login and registration diagram comes first. Break down report and service request activity diagram. Service provider and dispatch diagram. 

**Integration**

Taken four of these UML diagrams provide a complete blueprint and picture on working with FixMyRide from different perspectives and technicalities.

### **3.4 Team Roles and Responsibilities** {#3.4-team-roles-and-responsibilities}

### **Table 9: *Team roles and responsibilities*** {#table-9:-team-roles-and-responsibilities}

| Team member (UoW ID) | Agile role(s) | Main responsibilities |
| :---: | :---: | :---: |
| Aarshidan (W21823435) | Scrum Master & Developer | Sprint management and Prototype building |
| Vyshali (w2120032) | Product Owner & Developer | Project Requirements analysis and Diagrams |
| Dawood (w2182332) | Developer | Ethical analysis and presentation projector |
| Vithushan (w2149550) | Developer | GAP analysis and presentation projector |
| Safry (w2151085) | Developer | Overview, outside info and landing page  |

## **3.5 Sprint Structure and Agile Ceremonies** {#3.5-sprint-structure-and-agile-ceremonies}

### **3.5.1 Sprint Structure and Ceremonies** {#3.5.1-sprint-structure-and-ceremonies}

Sprints lasted- 29/10/2026 \- 22/11/2026

Recorded Sprints and tasks were done in individual word docs and meeting notes, which are implemented in the shared document.

Actual task start and implementation lasted \- 20/11/2026 \- 23/112026

Using task tracker and backlog, task progress and completion were recorded by our leader and members

### **3.5.2 Definition of Ready and Definition of Done** {#3.5.2-definition-of-ready-and-definition-of-done}

The definition of Ready is enough documentation is present to see a clear idea about the sprint. Done is when all the feedback related improvements were made.

### **3.5.3 Team Working Agreement** {#3.5.3-team-working-agreement}

Physical meetings after lectures and online meetings once a week and group calls were made. Physical meetings and combined working tasks were assigned for flexibility. Meeting tools like google calendar, zoom meetings and whatsapp group chat and calls were used to ease communication.

## **3.6 Tools and Version Control Workflow** {#3.6-tools-and-version-control-workflow}

| *Provide evidence (screenshots) of the tools used. For example:* *Task board for backlog and sprint management (Jira / Trello / GitHub Projects)* *Git repository with the agreed branching strategy (e.g. feature branches, pull requests and code reviews)* *Communication and collaboration (Slack / Discord / Teams)* *Design and prototyping tools (Figma / Balsamiq)* *Summarise the tools in a table showing the purpose, the tool and how the team actually used it.* |
| :---- |

**Table** 10**:** *Tools used by the team*

| Purpose | Tool | How the team used it |
| ----- | ----- | ----- |
| Backlog and task board | Jiraa |  |
| Version control | Github and google document |  |
| Communication | Google Meetings, Whatsapp, gmail, zoom |  |
| Design and prototyping | figma |  |
| Testing |  |  |

## **3.7 Communication Plan** {#3.7-communication-plan}

| *How the team communicates internally and with the client and supervisor, including the weekly meeting log. Include the meeting log template here and the completed logs in the appendix (Appendix B).* |
| :---- |

**Table** 11**:** *Meeting log template*

| Meeting type | Team / Supervisor / Client |
| :---- | :---- |
| **Date, time and venue** |  |
| **Attendees and apologies** |  |
| **Agenda** |  |
| **Key discussion points** |  |
| **Decisions made** |  |
| **Action items (owner and due date)** |  |
| **Next meeting** |  |

## **3.8 User Needs and Requirements Definition** {#3.8-user-needs-and-requirements-definition}

### **3.8.1 User Personas** {#3.8.1-user-personas}

| *Describe the main user groups as personas, based on the stakeholders in Chapter 4 and the elicitation results. Create one persona per key user group using the template below.* |
| :---- |

**Table** 20**:** *User persona template*

| Persona name and photo / avatar |  |
| :---- | :---- |
| **Age, occupation and background** |  |
| **Goals and needs** |  |
| **Pain points and frustrations** |  |
| **Technology use and skills** |  |
| **Linked stakeholder group** |  |

### **3.8.2 User Stories** {#3.8.2-user-stories}

| *Express the requirements as user stories in the form “As a \[persona\], I want \[feature\], so that \[benefit\]”. Each story must be linked to its functional requirement (Section 4.7) and persona, estimated in story points, and have acceptance criteria.* *Priority (MoSCoW) and target sprint are managed in the product backlog (Section 3.7).* |
| :---- |

**Table** 21**:** *User stories with estimates and acceptance criteria*

| ID | Persona | User story (As a… I want… so that…) | Estimate (story points) | Acceptance criteria |
| ----- | ----- | ----- | ----- | ----- |
| US1 |  |  |  |  |
| US2 |  |  |  |  |
| US3 |  |  |  |  |

## **3.9 Product Backlog** {#3.9-product-backlog}

| *The product backlog is the single, ordered list of everything the product needs. It is maintained throughout the project and is kept separate from the requirements chapter so that its management is shown as part of the team’s Agile practice.* |
| :---- |

### **3.9.1 Backlog Creation and Prioritisation** {#3.9.1-backlog-creation-and-prioritisation}

| *Explain how the backlog was created, how items are prioritised using MoSCoW (Must have, Should have, Could have, Won’t have this time), and how it is refined each sprint using client and supervisor feedback.* *Each backlog item is a user story (Section 6.4.2) traced to a functional requirement (Section 4.7). Story point estimates are recorded against each user story in Section 6.4.2 and are not repeated here.* |
| :---- |

### **3.9.2 Prioritised Product Backlog** {#3.9.2-prioritised-product-backlog}

**Table** 12**:** *Prioritised product backlog*

| Rank | User story | Backlog item | Priority (MoSCoW) | Target sprint | Status |
| ----- | ----- | ----- | ----- | ----- | ----- |
| 1 |  |  |  |  |  |
| 2 |  |  |  |  |  |
| 3 |  |  |  |  |  |

### **3.9.3 Task Board Evidence** {#3.9.3-task-board-evidence}

| *The backlog must also be maintained on the team’s task board. Include a screenshot of the board showing the backlog.* |
| :---- |

## **3.10 Release Plan / Roadmap** {#3.10-release-plan-/-roadmap}

**Table** 13**:** *Release plan for Sprints 0 to 4*

| Sprint | Dates | Sprint goal | Major milestone |
| ----- | ----- | ----- | ----- |
| Sprint 0 | 19/10/2026 \- 29/112026 | Idea was to be  found and GAP analysis for it  | GAP analysis and requirements were observed.  |
| Sprint 1 | 29/11/2026 \- 5/11/2026 | Gap analysis and new idea overview | Mechanic idea was chose, Gap analysis was done, with responses and reviews of apps  |
| Sprint 2 | 5/11/2026 \- 12/11/2026 | Tools to be used | Tools were done, and project overview was done |
| Sprint 3 | 12/11/2026-23/112026 | Task completion and documentation | Documents was satisfactory |

## **3.11 Risks and MitigationTable 14: *Risk register*** {#3.11-risks-and-mitigationtable-14:-risk-register}

| Risk item | Severity | Frequency | Mitigation plan |
| ----- | :---: | :---: | ----- |
| Security breaches  | high | mid | Implement security tools and services. |

## **3.12 Chapter Summary** {#3.12-chapter-summary}

| *This is a small summary of your chapter.* |
| :---- |

# Chapter 4: System Requirements Specification (SRS) {#chapter-4:-system-requirements-specification-(srs)}

## **4.1 Chapter Overview** {#4.1-chapter-overview}

This chapter describes the System Requirements Specification (SRS) of the proposed Location-Based Roadside Assistance and Vehicle Parts Finder System. It identifies the stakeholders, their expectations, and the requirements of the proposed system.

The main purpose of the system is to help drivers who experience unexpected vehicle breakdowns find nearby available mechanics through GPS-based location services. The system allows drivers to share their live GPS locations with mechanics and communicate directly with them.

Furthermore, the system provides a vehicle hardware store finder feature that allows both drivers and mechanics to locate nearby hardware stores and search available spare-parts inventory.

This chapter includes stakeholder analysis, requirement elicitation techniques, discussion and analysis of elicitation results, use case diagrams, use case descriptions, functional requirements, non-functional requirements, and assumptions and clarifications. 

## 

## **4.2 Stakeholder Analysis** {#4.2-stakeholder-analysis}

analysis identifies the individuals, groups, and external systems that interact with or are affected by the proposed system.

The main stakeholders of the proposed system include drivers, mechanics, vehicle hardware store owners and staff, GPS services, and other supporting stakeholders.

Stakeholders are classified into direct and indirect stakeholders according to their interaction with the proposed system.

## 

## 

## 

## **4.2.1 Onion Model** {#4.2.1-onion-model}

![][image1]

**Figure** 2**:**  *onion diagram*

### **4.2.2 Stakeholder Descriptions** {#4.2.2-stakeholder-descriptions}

**Table** 15**:** *Stakeholder descriptions*

| Stakeholder | Viewpoint |
| ----- | ----- |
| **Functional beneficiary** |  Drivers use the system to find nearby mechanics, share live GPS locations, communicate with mechanics, and search spare parts. Mechanics use the system to find drivers, view shared locations, communicate with drivers, and search spare-parts inventory  |
| **Financial beneficiary** | Mechanics may benefit from increased opportunities to connect with drivers requiring roadside assistance. Vehicle hardware store owners may benefit from increased visibility of their stores and products.  |
| **Social beneficiary** | Drivers can receive easier access to roadside assistance during unexpected vehicle breakdowns. Mechanics can improve communication with drivers, while vehicle owners benefit from easier access to spare-parts information  |
| **Operational beneficiary** | Hardware store owners and staff may provide and maintain store and inventory information. The system administrator manages user and system information.    |
| **Negative stakeholders** | Users may experience difficulties when GPS information is inaccurate, internet connectivity is unavailable, or location information is misused.  |
| **Regulatory** | Relevant data protection, privacy, and consumer protection authorities may influence how personal information and location data are handled  |
| **Experts** | Automobile mechanics, vehicle spare-parts specialists, GPS and mapping specialists, and software engineering experts.  |
| **Neighbouring systems** | GPS and mapping services, internet services, external communication services, and other systems providing location or inventory information.  |

## 

## **4.3 Selection of Requirement Elicitation Techniques / Methods** {#4.3-selection-of-requirement-elicitation-techniques-/-methods}

**01.Online Questionnaire Survey**

An online questionnaire was created using Google Forms and distributed among vehicle owners, drivers, and mechanics to collect information about their vehicle breakdown experiences and expectations regarding the proposed application.

The questionnaire mainly focused on:

* Common vehicle breakdowns experienced by drivers.  
* Problems faced when searching for roadside assistance.  
* Features users and mechanics would prefer in the application.  
* Benefits of developing a roadside assistance application.  
* Suggestions for improving roadside assistance services.


Some of the common vehicle breakdown categories included flat or damaged tyres, engine overheating, fuel-related problems, and dead or weak batteries.

This method helped the development team collect information from different participants and understand their expectations regarding the proposed system.

**02\. Informal Discussions with Mechanics and Vehicle Users**

Informal discussions were conducted through telephone calls with some mechanics and individuals who had experienced vehicle breakdowns.

These discussions helped the development team understand practical problems associated with roadside assistance services and the challenges faced by both customers and mechanics.

The discussions mainly focused on:

* Common problems experienced during vehicle breakdowns.  
* Difficulties in finding nearby mechanics.  
* Challenges mechanics experience when providing roadside assistance.  
* Delays in receiving repair services.  
* Difficulties in identifying vehicle problems.  
* Possible improvements to roadside assistance services.

**03\. Observation of Existing Roadside Assistance Practices**

The development team considered existing roadside assistance practices and vehicle breakdown situations to understand the challenges faced by vehicle owners when seeking repair services.

The main areas considered included:

* Difficulties faced by drivers when their vehicles break down.  
* Challenges in identifying suitable mechanics.  
* The process of communicating vehicle problems to mechanics.  
* The importance of sharing accurate customer locations.  
* The need for quick and reliable roadside assistance.

This approach helped the development team understand the importance of providing a simple and user-friendly system that connects customers with nearby mechanics and other roadside assistance service providers.

The findings helped identify potential improvements and supported the design of the proposed fix my ride application.

## 

## **4.4 Discussion / Analysis of Results** {#4.4-discussion-/-analysis-of-results}

This section discusses and analyses the information collected through the selected requirement elicitation techniques. The findings helped the development team understand existing roadside assistance problems and identify the necessary features and functional requirements for the proposed fix my ride application.

**4.4.1 Analysis of Online Questionnaire Survey**

The online questionnaire survey provided useful information about vehicle breakdown experiences, user expectations, and preferred features of the proposed application.

The collected responses highlighted several common vehicle breakdown problems, including:

* Flat or damaged tyres.  
* Engine overheating.  
* Fuel-related problems.  
* Dead or weak batteries.  
* Other unexpected vehicle failures.

The responses also highlighted the difficulties experienced by vehicle owners when searching for suitable roadside assistance during unexpected breakdown situations.

Furthermore, participants were asked about the additional features they would prefer in the application. Their responses helped the development team identify the importance of providing a convenient platform for connecting customers with mechanics.

Based on the collected information, the following features were identified as important considerations:

* Real-Time GPS Location Sharing.  
* Nearby Service Provider Search.  
* Real-Time Mechanic Tracking.  
* Emergency SOS.  
* Push Notifications.  
* In-App Communication.


These findings helped the development team identify the major functional requirements of the proposed application.

**4.4.2 Analysis of Informal Discussions**

The informal telephone discussions with mechanics and individuals who had experienced vehicle breakdowns provided additional practical insights into the existing roadside assistance process.

The discussions helped the development team understand the difficulties involved in identifying vehicle problems, locating available mechanics, and providing timely assistance to customers.

The information highlighted the importance of improving communication between customers and mechanics and making it easier for mechanics to identify customer locations.

Based on these discussions, the development team identified the following requirements:

* Customers should be able to request roadside assistance easily.  
* Customers should be able to share their current GPS location with mechanics.  
* Mechanics should be able to view customer locations and service requests.  
* Customers should be able to communicate with mechanics.  
* The system should provide updates about service request progress.  
* Mechanics should be able to manage and respond to customer requests.  
* 

These findings supported the inclusion of GPS-based location sharing, mechanic searching, service request management, real-time tracking, and communication features.

**4.4.3 Analysis of Observation Findings**

The consideration of existing roadside assistance practices helped the development team understand the difficulties experienced by drivers during vehicle breakdown situations.

The findings highlighted the importance of providing an easy way to request assistance, identifying nearby service providers, and sharing accurate location information.

As a result, the proposed fix my ride application aims to provide:

* A simplified roadside assistance request process.  
* GPS-based customer location sharing.  
* Nearby mechanic searching.  
* Real-time tracking of mechanics.  
* Emergency SOS functionality.  
* Improved communication between customers and mechanics.

These findings influenced the proposed system design and helped the development team identify features that could improve the roadside assistance experience.

 

 

## **4.5 Use Case Diagram** {#4.5-use-case-diagram}

## **![][image2]**

## **4.6 Use Case Descriptions** {#4.6-use-case-descriptions}

| *Use the following template for the use case descriptions.* |
| :---- |

**Table** 16**:** *Use case description* 

| Use Case Name | Register/Login |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC1** |  |
| **Description** | Allows users to create an account or log in to the FixMyRide system  |  |
| **Priority** | High |  |
| **Primary Actor** | Customer |  |
| **Supporting Actors** | None |  |
| **Pre-Conditions** | Users must have access to the application.  |  |
| **Trigger** | User selects the Register or Login option  |  |
| **Main flow** | **Actors** | **System** |
|  | User opens the application  User selects Register.  User enters personal details  User submits the details  User selects Login and enters credentials  | Displays Register and Login options.  Displays the registration form. Validates the entered information.   Creates the user account.  Authenticates the user and grants access.  |
| **Exception flow** | **Actors** | **System** |
|  | The user enters incorrect information.  The user enters an already registered email.  | Displays an error message.  Displays an account already exists message.  |
| **Alternate flow** | **Actors** | **System** |
|  | Existing user selects Login directly  The user enters valid credentials.  | Displays the login form.  Authenticates the user and opens the account.  |
| **Exclusions** |  |  |
| **Post-Conditions** | User successfully register or logs into the system.  |  |

| Use Case Name | Manage Profile  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC2** |  |
| **Description** | Allows users to view and update their personal profile information.  |  |
| **Priority** | High |  |
| **Primary Actor** | Customer, Mechanic, Hardware Store Owner/Staff  |  |
| **Supporting Actors** | None |  |
| **Pre-Conditions** | The user must be registered and logged in.  |  |
| **Trigger** | The user selects the Manage Profile option.  |  |
| **Main flow** | **Actors** | **System** |
|  | 1\. The user opens the profile section. 2\. The user views existing details.  3\. The user edits the required information. 4\. The user saves the changes.  | 1\. Displays the user's profile. 2\. Allows profile information to be edited.  3\. Validates the updated information.  4\. Save the changes.  |
| **Exception flow** | **Actors** | **System** |
|  | User enters invalid or incomplete information  | Displays validation messages and requests corrections.  |
| **Alternate flow** | **Actors** | **System** |
|  | The user views the profile without making changes.  | Displays the existing profile information.  |
| **Exclusions** |  |  |
| **Post-Conditions** | The profile information is updated or remains unchanged.  |  |

| Use Case Name | Search Nearby Service Providers  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC3** |  |
| **Description** | Allows customers to search for nearby mechanics or vehicle repair service providers based on their current location.  |  |
| **Priority** | High |  |
| **Primary Actor** | Customer |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** | The customer must be logged in and location access should be available.  |  |
| **Trigger** | Customer selects Search Nearby Service Providers.  |  |
| **Main flow** | **Actors** | **System** |
|  | 1\. The customer opens the search option.  2\. Customers allow location access.  3\. Customer searches for nearby service providers.  | 1\. Retrieves the customer's current location.  2\. Identifies nearby service providers.  3\. Displays available providers and their locations.  |
| **Exception flow** | **Actors** | **System** |
|  | Customer denies location permission.  | Displays a message requesting location permission or allows manual location entry if supported.  |
| **Alternate flow** | **Actors** | **System** |
|  | The customer enters a location manually.  | Displays service providers near the entered location.  |
| **Exclusions** |  |  |
| **Post-Conditions** | Nearby service providers are displayed to the customer.  |  |

| Use Case Name | View Mechanic Details  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC4** |  |
| **Description** | Allows customers to view mechanic information such as name, contact details, services, experience and availability.  |  |
| **Priority** | High  |  |
| **Primary Actor** | Customer  |  |
| **Supporting Actors** | None |  |
| **Pre-Conditions** | Customer must be logged in and mechanic details must be available  |  |
| **Trigger** | Customer selects a mechanic from the search results.  |  |
| **Main flow** | **Actors** | **System** |
|  | 1\. The customer selects a mechanic.  2\. Customer requests to view mechanic details.  | 1\. Retrieves the selected mechanic's information.  2\. Displays the mechanic's profile, services and availability details.  |
| **Exception flow** | **Actors** | **System** |
|  | Customer selects a mechanic whose profile is unavailable.  | Displays a message that the mechanic's details cannot be retrieved.  |
| **Alternate flow** | **Actors** | **System** |
|  | The customer selects another mechanic.  | Displays the selected mechanic's details.  |
| **Exclusions** |  |  |
| **Post-Conditions** | The selected mechanic's details are displayed.  |  |

| Use Case Name | Get Current GPS Location  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC5** |  |
| **Description** | Retrieves the customer's current geographical location using GPS to support nearby service searches and location sharing.  |  |
| **Priority** | High |  |
| **Primary Actor** | Customer  |  |
| **Supporting Actors** | GPS / Location Service  |  |
| **Pre-Conditions** | The customer must be using the system and the device must support location services  |  |
| **Trigger** | The customer selects an option that requires their current location.  |  |
| **Main flow** | **Actors** | **System** |
|  | 1\. The customer selects the location option.  2\. Customer grants location permission.  | 1\. Requests the current location from the GPS service. 2\. Receives the location coordinates.  3\. Displays or stores the retrieved location for the requested operation.  |
| **Exception flow** | **Actors** | **System** |
|  | The customer denies GPS permission or the device location is unavailable.  | Displays a location access error message.  |
| **Alternate flow** | **Actors** | **System** |
|  | Customer enters the location manually | Uses the manually entered location for the relevant operation.  |
| **Exclusions** | Continuous mechanic tracking and navigation.  |  |
| **Post-Conditions** | The customer's current location is retrieved or an error is displayed.  |  |

| Use Case Name | Request Mobile Mechanic  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** | Allows customers to request a mechanic to visit their location to repair their vehicle.  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

| Use Case Name |  |  |
| :---- | :---- | :---- |
| **Use Case ID** | **UC-001** |  |
| **Description** |  |  |
| **Priority** |  |  |
| **Primary Actor** |  |  |
| **Supporting Actors** |  |  |
| **Pre-Conditions** |  |  |
| **Trigger** |  |  |
| **Main flow** | **Actors** | **System** |
|  |  |  |
| **Exception flow** | **Actors** | **System** |
|  |  |  |
| **Alternate flow** | **Actors** | **System** |
|  |  |  |
| **Exclusions** |  |  |
| **Post-Conditions** |  |  |

## 

## 

## 

## **4.7 Functional Requirements** {#4.7-functional-requirements}

## **Table 17: *Functional requirements*** {#table-17:-functional-requirements}

| ID | Functional requirement | Source |
| ----- | ----- | ----- |
| FR1 | The system shall allow drivers to register and log in  | Client/Project requirements  |
| FR2 | The system shall allow mechanics to register and log in  | Client/Project requirement  |
| FR3 | The system shall allow drivers and mechanics to manage their profiles   | Stakeholders requirements   |
| FR4 | The system shall allow mechanics to update their availability status | Mechanic requirements  |
| FR5 | The system shall allow drivers to search for nearby mechanics  | Client requirements  |
| FR6 | The system shall identify nearby available mechanics using GPS location information  | Client requirements |
| FR7 | The system shall allow drivers to share their live GPS location with selected mechanics  | Client requirements |
| FR8 | The system shall allow mechanics to view locations shared by drivers  | Client requirements |
| FR9 | The system shall allow drivers and mechanics to communicate directly  | Client requirements |
| FR10 | The system shall allow drivers to find nearby vehicle hardware stores  | Project requirements  |
| FR11 | The system shall allow mechanics to find nearby vehicle hardware stores  | Project requirements |
| FR12 | The system shall allow drivers to search spare parts inventory  | Project requirements |
| FR13 | The system shall allow mechanics to search spare parts inventory  | Project requirements |
| FR14 | The system shall display matching spare parts information and availability  | Stakeholder requirements  |
| FR15 | The system shall display relevant hardware store information | Stakeholder requirements  |

## **4.8 Non-Functional Requirements** {#4.8-non-functional-requirements}

## **Table 18: *Non-functional requirements*** {#table-18:-non-functional-requirements}

| ID | Category | Requirement | Priority | How measured / tested |
| ----- | ----- | ----- | ----- | ----- |
| NFR1 | Performance | The system should display search results within five seconds under normal network conditions  | High | Measure search response time during testing  |
| NFR2 | Security | The system shall protect user accounts through secure authentication  | High | Test login and unauthorized access attempts |
| NFR3 | Data Protection  | The system shall prevent unauthorized access to personal and location information   | High  | Conduct access control and privacy tests  |
| NFR4 | Usability | The system should provide a simple and user friendly interface  | High | Conduct usability testing with potential users  |
| NFR5 | reliability | The system should provide reliable search and communication services when required external services are available  | High  | Conduct functional and reliability testing  |
| NFR6 | Location Accuracy | The system should use available GPS information to identify nearby mechanics and hardware stores accurately | High | Compare displayed locations with actual test locations  |
| NFR7 | Availability | The system should be accessible when the application server and internet connection are available  | Medium | Conduct availability testing  |
| NFR8 | Accessibility | The application should provide readable text,clear,labels and understandable navigation  | Medium  | Conduct accessibility and interface testing |
| NFR9 | Compatibility | The web application should work with commonly used modern web browsers  | Medium  | Test across different browsers and screen sizes  |
| NFR10 | Sustainability | The system should avoid unnecessary GPS updates and network requests to reduce resource consumption  | medium | Monitor location updates and network usage  |

## **4.9 Assumptions and Clarifications** {#4.9-assumptions-and-clarifications}

## **Table 19: *Assumptions and clarifications*** {#table-19:-assumptions-and-clarifications}

| Ref | Ambiguity or gap | Assumption made or question asked | Outcome |
| ----- | ----- | ----- | ----- |
| AS1 | How will the system identify nearby mechanics? | The system is expected to use GPS based location services  | Nearby mechanics search will use location information  |
| AS2 | How will drivers share their locations? | Drivers will be able to share their live GPS locations with selected mechanics after granting permission   | Live location sharing is included in the proposed scope  |
| AS3 | How will drivers and mechanics communicate? | The system will provide a direct communication feature. The exact method needs client confirmation. | Communication is included; implementation method must be confirmed  |
| AS4 | How will mechanical availability be displayed? | Mechanics will be able to update their availability status. | Availability information is included in proposed scope |
| AS5 | How will spare parts information be updated? | Hardware store owners or staff will provide accurate store and inventory information | The inventory update process needs client confirmation  |
| AS6 | Can both drivers and mechanics search for spare parts? | Both user groups will be allowed to search available spare parts inventory  | Confirmed as part of the agreed project scope  |
| AS7 | Will the system include booking management? | The system will focus on locating mechanics and direct communication rather than booking acceptance or rejection  | Booking management is excluded  |
|  AS8 | Will the system include repair progress tracking? | The system will not manage or track repair progress  | Repair progress tracking is excluded |
| AS9 | Will the system support online spare parts purchasing?  | The system will focus on locating stores and searching inventory rather than online purchasing  | Online purchasing and payment are excluded  |
| AS10 | What happens if GPS or internet connectivity is unavailable? | The system requires location and internet services for its location based features. | An appropriate error message should be displayed when services are unavailable  |

## 

## 

## **4.10 Chapter Summary** {#4.10-chapter-summary}

The chapter identified the main stakeholders, including drivers, mechanics, vehicle hardware store owners, and external service providers. The Onion Model and stakeholder descriptions were used to explain their relationships with the proposed system.

Furthermore, suitable requirement elicitation techniques were identified, and the expected results were analyzed. The use case diagram and use case descriptions explained how different actors interact with the system.

Finally, the functional and non-functional requirements were documented, together with the assumptions and clarifications related to the proposed system.

These requirements provide a foundation for the system design and development activities in the following chapter 

# Chapter 5: Social, Legal, Ethical and Professional Issues {#chapter-5:-social,-legal,-ethical-and-professional-issues}

## **5.1 Chapter Overview** {#5.1-chapter-overview}

In this chapter the social, legal, ethical and professional issues of FixMyRide are explained. FixMyRide is an app which helps drivers in Sri Lanka to find verified mechanics and garages. It also allows drivers to call and text mechanics and search for parts,send an emergency SOS, get chatbot help. The chapter examines ethical clearance and six issue groups. Each group has a fix that is related to BCS Code of Conduct (BCS, 2022).

## **5.2 Ethical Clearance** {#5.2-ethical-clearance}

| *Clear evidence of ethical clearance should be provided. If a dataset is downloaded from any data repository (e.g. Kaggle), you should also include proper citation along with the license information. Should fill the UoW Ethics form A and form B if needed.* |
| :---- |

## 

## **5.3 SLEP Issues and Mitigation** {#5.3-slep-issues-and-mitigation}

# 

# 5.3.1 Legal Issues  {#5.3.1-legal-issues}

* ***Legal** – data protection (UK GDPR and Sri Lanka’s Personal Data Protection Act No, intellectual property and software licensing.*

- The app uses personal data such as names,phone numbers and the driver’s location to find nearby providers, so it must follow Sri Lanka’s person Act No.9 of 2022(Sri Lanka, 2022\)  and the UK GDPR (UK Government, 2018).

| Issue  | How we handle it  | BCS Core Principles |
| :---- | :---- | :---- |
| Personal data  | Collect only what is needed.Publish a privacy notice. Let users edit or delete their data. | Public Interest, Duty to Relevant Authority  |
| Live Location Sharing | A driver's location is shared only with the mechanic they choose, only after they agree and only while the job is active. Sharing stops when the job ends and the location history is then deleted. | Public Interest, Duty to Relevant Authority |
| Tracking of mechanics | A mechanic's location is shown only while they are online and on a job a driver has chosen. Mechanics can go offline at any time. | Public Interest  Professional Competence and Integrity |
| Contact details | Providers show business contact details only.A drivers phone number is shared only when the driver chooses to message a provider or pre-order a part.  | Public Interest, Duty to Relevant Authority |
| Garage stock data | Garages own their data and can edit or delete it. No copying from other websites  | Professional Competence and Integrity, Duty to Relevant Authority  |
| Part pre-order | Show "last updated" times on stock and prices and state that the garage is the seller. Payment and refunds are handled directly with the garage, not through the app.  | Public Interest, Professional Competence and Integrity.  |
| Licensing  | Use an open-source licence and follow map and library terms .  | Professional Competence and Integrity. Duty to the profession. |

# 5.3.2 Ethical issues  {#5.3.2-ethical-issues}

• ***Ethical** – privacy, consent, bias and the needs of others* 

- Drivers are often stressed after a breakdown, so the design focuses on trust, safety and fairness. The app only connects people; the mechanic or garage does the work.

| Issue  | How we handle it  | BCS Core Principles |
| :---- | :---- | :---- |
| Fake Providers  | Admins verify mechanics and garages before they appear.  | Professional Competence and Integrity, Public Interest  |
| Quality of work | The app does not guarantee any repair, and says clearly.Ratings help drivers choose. | Professional Competence and Integrity, Public Interest  |
| Wrong or fake parts  | Match parts to the vehicle,show their condition and lets users report problems | Professional Competence and Integrity, Public Interest  |
| Fake or unfair reviews | Reviews only from registered users, one per provider, with a report option and a right of reply for providers. | Professional Competence and Integrity, Public Interest  |
| Emergency SOS  | The SOS alert goes only to the people the driver chooses. It is not a replacement for emergency services, so the app also shows numbers such as 119, and alerts can be cancelled to avoid false alarms. | Public Interest |
| Chatbot answers  | The chatbot is labelled as automated, can be wrong, and gives no safety-critical repair advice. It points users to a verified mechanic instead. | Public Interest, Professional Competence and Integrity |
| Fairness | Rank by distance and rating not by payment. | Public Interest |

# 5.3.3  Security Issue  {#5.3.3-security-issue}

*• **Security** – how security is built into the design and each sprint* 

- Security is checked in every sprint and follows the OWASP Top 10 (OWASP, 2021).

| Risk | How we handle it | BCS Core Principles |
| :---- | :---- | :---- |
| Stolen Accounts  | Hashed passwords and token-based login.  | *Professional Competence and Integrity, Public Interest*  |
| Data Interception  | HTTPS and encrypted database fields | *Professional Competence and Integrity,* |
| Wrong access  | Role-based access for drivers, providers and admins, and users can change only their own data. | Public Interest |
| Misuse of live location  | Location is sent only over encrypted connections,is visible only to the chosen mechanic, and is deleted after the job | Public Interest, Professional Competence and Integrity |
| Fake stock or orders  | Only verified garages edit their own listings, and changes are logged | *Professional Competence and Integrity,* |

# 

# 5.3.4 Equality, Diversity and Inclusion {#5.3.4-equality,-diversity-and-inclusion}

***• Equality, diversity and inclusion** – accessibility and inclusive design* 

- The app must work for people with different abilities, languages and network quality.

| Issue | How we handle it | BCS Core Principles |
| :---- | :---- | :---- |
| Accessibility | Follow WCAG 2.1 AA: good contrast, scalable text and screen-reader labels (W3C, 2018).  | Public Interest |
| Language | Sinhala, Tamil and English, with icons for parts and faults.  | Public Interest |
| Emergency use | The SOS and help screens use few steps,large buttons and icons so they work under stress. | Public Interest |
| Weak Signal | Light screens and a clear message when offline .  | Public Interest |
| Small garages | Free and simple sign-up and stock updates.  | Public Interest, Duty to the Profession  |

# 

# 

# 5.3.5 Sustainability  {#5.3.5-sustainability}

| Aspects | How we support it  |
| :---- | :---- |
| Environmental  | Accurate stock information means fewer wasted trips |
| Social | Supports local and rural garages and keeps drivers safer |
| Technical | Modular, open-source, documented and scalable designs(NFR06) |

# 5.3.6 Professional Issues  {#5.3.6-professional-issues}

| Issue  | How we handle it | BCS Core Principles |
| :---- | :---- | :---- |
| Teamwork | Tasks were shared fairly and contributions were recorded in Chapter 8\.  | Professional Competence and Integrity , Duty to the Profession |
| Handling disagreements  | The team followed its working agreement. | Professional Competence and Integrity , Duty to the Profession |

## **5.4 Chapter Summary** {#5.4-chapter-summary}

FixMyRide connects drivers with mechanics, garages and spare parts and handles live location,SOS alerts and chatbot help, so trust, privacy, safety and fairness are the main concerns. They are handled through verified providers, limited use of location and contact details, clear information, secure design and inclusive, sustainable choices.

# Chapter 6: System Architecture and Design {#chapter-6:-system-architecture-and-design}

## **6.1 Chapter Overview** {#6.1-chapter-overview}

This chapter focuses on the system architecture and design of FixMyRide. It explains how the main components of the application are organized and how they work together to provide the required services. The chapter includes the system architecture, system design diagrams, user interface wireframes, and prototype design. It also discusses the design principles and decisions considered to make the application simple, user friendly and suitable for its intended users.

## **6.2 System Architecture Design** {#6.2-system-architecture-design}

FixMyRide uses a layered architecture to organise the different components of the system. The architecture separates the application users, mobile application, backend processing, data storage and external services into five main layers. Each layer has its own responsibilities and communicates with other layers to provide the required system functionality.  
The Application Users layer represents the general public, mechanics and hardware shop owners. The Flutter Mobile Application Layer provides the user interfaces and main application features. The Spring Boot Backend Layer handles business logic and process requests through REST APIs. The Data and Storage Layer manages application information and uploaded files using MongoDB and Firebase services. Finally, the External Services Layer provides additional functionality through Firebase Authentication, Firebase Cloud Messaging and Google Maps Platform.  
This architecture provides  a clear structure for FixMyRide and shows how its main components interact to support the application’s features.

![][image3]

## **6.3 System Design** {#6.3-system-design}

| *Depending on the system, add appropriate design diagrams such as the following.* |
| :---- |

### **6.3.1 Class Diagram / Data Flow Diagram (DFD)** {#6.3.1-class-diagram-/-data-flow-diagram-(dfd)}

| *Add the class diagram or data flow diagram that best describes the system. Select based on your design methodology.*  |
| :---- |

### **6.3.2 Sequence Diagram** {#6.3.2-sequence-diagram}

| *Add sequence diagrams for the key interactions.* |
| :---- |

### **6.3.3 Activity Diagram** {#6.3.3-activity-diagram}

| *Add activity diagrams for the key workflows.* |
| :---- |

## **6.4 User-Centred Design and UI/UX** {#6.4-user-centred-design-and-ui/ux}

| *This section brings together the user-focused design work: who the users are, what they need, and how the interface was designed and tested with them. The subsections follow the order in which the work is normally done.* |
| :---- |

### **6.4.1 Wireframes** {#6.4.1-wireframes}

| *Include low-fidelity wireframes for the main screens and user flows. Show how the wireframes meet the needs of the personas and user stories above.* |
| :---- |

### **6.4.2 UI/UX (Figma)** {#6.4.2-ui/ux-(figma)}

| *Include the clickable high-fidelity prototype (e.g. Figma) and the prototype link. Explain the usability and accessibility considerations behind the design, and record the client feedback received on the prototype and the changes it led to.* |
| :---- |

**Table** 22**:** *Client feedback on the prototype*

| Feedback received | Date | Change made |
| ----- | ----- | ----- |
|  |  |  |
|  |  |  |

## **6.5 Design Principles and Sustainability** {#6.5-design-principles-and-sustainability}

| *Justify the design decisions made (e.g. separation of concerns, modularity, reusability, security by design) and how the design supports a sustainable, maintainable solution.* *Record the main design decisions in a table: the decision, the options considered and the reason for the choice.* |
| :---- |

**Table** 23**:** *Main design decisions*

| Decision | Options considered | Reason for the choice |
| ----- | ----- | ----- |
|  |  |  |
|  |  |  |

## **6.6 Chapter Summary** {#6.6-chapter-summary}

| *This is a small summary of your chapter.* |
| :---- |

# Chapter 7: Sprint Records {#chapter-7:-sprint-records}

## **7.1 Chapter Overview** {#7.1-chapter-overview}

| *This is a small introduction to your chapter.* |
| :---- |

This chapter records every sprint of the project, from Sprint 0 to Sprint 4, in one place. One record is completed per sprint using the same structure each time. Sprint 0 and Sprint 1 are delivered in Semester 1 and are fully recorded in Submission 1\. Sprints 2 – 4 are delivered in Semester 2; for Submission 1 only their goal, dates and planned backlog are completed.

**Table** 24**:** *Sprint overview*

| Sprint | Title | Semester | Status in Submission 1 |
| ----- | ----- | ----- | ----- |
| Sprint 0 | Inception and Set-up | Semester 1 | Delivered – full record |
| Sprint 1 | Requirements and Design Increment | Semester 1 | Delivered – full record |
| Sprint 2 | \[Sprint title\] | Semester 1 | Planned – goal, dates and backlog |
| Sprint 3 | \[Sprint title\] | Semester 1 | Planned – goal, dates and backlog |
| Sprint 4 | \[Sprint title\] | Semester 1 | Planned – goal, dates and backlog |

Every sprint record uses the six sub-sections described below. Each sprint is numbered 7.x, so Sprint 0 is Section 7.2, Sprint 1 is Section 7.3, and so on.

**Table** 25**:** *Structure of each sprint record*

| Ref | Sub-section | What to include |
| ----- | ----- | ----- |
| 7.x.1 | **Sprint Goal and Dates** | The sprint goal and the start and end dates. |
| 7.x.2 | **Sprint Planning and Sprint Backlog** | The backlog items selected for the sprint, their estimates and owners (include a screenshot of the task board at sprint start). |
| 7.x.3 | **Stand-up and Progress Summary** | A summary of the stand-ups, blockers raised and how they were resolved, an events table, and a burndown or burnup chart with 3 – 5 sentences of interpretation. Detailed logs go in the appendix. |
| 7.x.4 | **Increment Delivered** | What was completed against the Definition of Done (for Sprint 1: requirements, design artefacts and prototype), with links to the repository, task board and prototype. |
| 7.x.5 | **Sprint Review and Feedback** | Feedback from the client, supervisor and users, and the changes it caused to priorities, scope or design. |
| 7.x.6 | **Sprint Retrospective** | What went well, what did not go well, and the improvement actions for the next sprint. Each retrospective must follow up on the actions agreed in the previous one. |

## **7.2 Sprint 0 – Inception and Set-up** {#7.2-sprint-0-–-inception-and-set-up}

### **7.2.1 Sprint Goal and Dates** {#7.2.1-sprint-goal-and-dates}

**Table** 26**:** *Sprint 0 goal and dates*

| Sprint goal |  |
| :---- | :---- |
| **Start date** |  |
| **End date** |  |

### **7.2.2 Sprint Planning and Sprint Backlog** {#7.2.2-sprint-planning-and-sprint-backlog}

| *Include a screenshot of the task board at sprint start. Estimates refer to the user stories in Section 6.4.2.* |
| :---- |

**Table** 27**:** *Sprint 0 backlog*

| Story | Task | Estimate | Owner | Status |
| ----- | ----- | ----- | ----- | ----- |
|  |  |  |  |  |
|  |  |  |  |  |

### **7.2.3 Stand-up and Progress Summary** {#7.2.3-stand-up-and-progress-summary}

| *Summarise the stand-ups, blockers raised and how they were resolved, with the burndown or burnup chart and 3 – 5 sentences interpreting it. Summarise each Agile event in the table below.* |
| :---- |

**Table** 28**:** *Sprint 0 Agile events*

| Agile event | Date | Participants | Outcomes | Evidence (Appendix E) |
| ----- | ----- | ----- | ----- | ----- |
| Sprint planning |  |  |  |  |
| Stand-ups |  |  |  |  |
| Sprint review |  |  |  |  |
| Retrospective |  |  |  |  |

### **7.2.4 Increment Delivered** {#7.2.4-increment-delivered}

| *What was completed against the Definition of Done, with links to the repository and task board.* |
| :---- |

### **7.2.5 Sprint Review and Feedback** {#7.2.5-sprint-review-and-feedback}

| *Feedback from the client, supervisor and users, and the changes it caused to priorities, scope or design.* |
| :---- |

### **7.2.6 Sprint Retrospective** {#7.2.6-sprint-retrospective}

| *What went well, what did not go well, and the improvement actions for the next sprint. Each retrospective must follow up on the actions agreed in the previous one.* |
| :---- |

**Table** 29**:** *Sprint 0 retrospective*

| What went well | What did not go well | Actions for next sprint (owner) |
| ----- | ----- | ----- |
|  |  |  |
|  |  |  |

## **7.3 Sprint 1 – Requirements and Design Increment** {#7.3-sprint-1-–-requirements-and-design-increment}

### **7.3.1 Sprint Goal and Dates** {#7.3.1-sprint-goal-and-dates}

**Table** 30**:** *Sprint 1 goal and dates*

| Sprint goal |  |
| :---- | :---- |
| **Start date** |  |
| **End date** |  |

### **7.3.2 Sprint Planning and Sprint Backlog** {#7.3.2-sprint-planning-and-sprint-backlog}

| *Include a screenshot of the task board at sprint start. Estimates refer to the user stories in Section 6.4.2.* |
| :---- |

**Table** 31**:** *Sprint 1 backlog*

| Story | Task | Estimate | Owner | Status |
| ----- | ----- | ----- | ----- | ----- |
|  |  |  |  |  |
|  |  |  |  |  |

### **7.3.3 Stand-up and Progress Summary** {#7.3.3-stand-up-and-progress-summary}

| *Summarise the stand-ups, blockers raised and how they were resolved, with the burndown or burnup chart and 3 – 5 sentences interpreting it. Summarise each Agile event in the table below.* |
| :---- |

**Table** 32**:** *Sprint 1 Agile events*

| Agile event | Date | Participants | Outcomes | Evidence (Appendix E) |
| ----- | ----- | ----- | ----- | ----- |
| Sprint planning |  |  |  |  |
| Stand-ups |  |  |  |  |
| Sprint review |  |  |  |  |
| Retrospective |  |  |  |  |

### **7.3.4 Increment Delivered** {#7.3.4-increment-delivered}

| *What was completed against the Definition of Done (requirements, design artefacts and prototype), with links to the repository, task board and prototype.* |
| :---- |

### **7.3.5 Sprint Review and Feedback** {#7.3.5-sprint-review-and-feedback}

| *Feedback from the client, supervisor and users, and the changes it caused to priorities, scope or design.* |
| :---- |

### **7.3.6 Sprint Retrospective** {#7.3.6-sprint-retrospective}

| *What went well, what did not go well, and the improvement actions for the next sprint. Each retrospective must follow up on the actions agreed in the previous one.* |
| :---- |

**Table** 33**:** *Sprint 1 retrospective*

| What went well | What did not go well | Actions for next sprint (owner) |
| ----- | ----- | ----- |
|  |  |  |
|  |  |  |

## **7.4 Sprint 2** {#7.4-sprint-2}

### **7.4.1 Sprint Goal and Dates** {#7.4.1-sprint-goal-and-dates}

**Table** 34**:** *Sprint 2 planned goal and dates*

| Sprint goal |  |
| :---- | :---- |
| **Start date** |  |
| **End date** |  |

### **7.4.2 Sprint Planning and Sprint Backlog** {#7.4.2-sprint-planning-and-sprint-backlog}

**Table** 35**:** *Sprint 2 planned backlog*

| Story | Task | Estimate | Owner | Status |
| ----- | ----- | ----- | ----- | ----- |
|  |  |  |  |  |
|  |  |  |  |  |

### **7.4.3 Stand-up and Progress Summary** {#7.4.3-stand-up-and-progress-summary}

| *To be completed in Semester 2 as Sprint 2 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

### **7.4.4 Increment Delivered** {#7.4.4-increment-delivered}

| *To be completed in Semester 2 as Sprint 2 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

### **7.4.5 Sprint Review and Feedback** {#7.4.5-sprint-review-and-feedback}

| *To be completed in Semester 2 as Sprint 2 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

### **7.4.6 Sprint Retrospective** {#7.4.6-sprint-retrospective}

| *To be completed in Semester 2 as Sprint 2 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

## **7.5 Sprint 3** {#7.5-sprint-3}

### **7.5.1 Sprint Goal and Dates** {#7.5.1-sprint-goal-and-dates}

**Table** 36**:** *Sprint 3 planned goal and dates*

| Sprint goal |  |
| :---- | :---- |
| **Start date** |  |
| **End date** |  |

### **7.5.2 Sprint Planning and Sprint Backlog** {#7.5.2-sprint-planning-and-sprint-backlog}

**Table** 37**:** *Sprint 3 planned backlog*

| Story | Task | Estimate | Owner | Status |
| ----- | ----- | ----- | ----- | ----- |
|  |  |  |  |  |
|  |  |  |  |  |

### **7.5.3 Stand-up and Progress Summary** {#7.5.3-stand-up-and-progress-summary}

| *To be completed in Semester 2 as Sprint 3 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

### **7.5.4 Increment Delivered** {#7.5.4-increment-delivered}

| *To be completed in Semester 2 as Sprint 3 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

### **7.5.5 Sprint Review and Feedback** {#7.5.5-sprint-review-and-feedback}

| *To be completed in Semester 2 as Sprint 3 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

### **7.5.6 Sprint Retrospective** {#7.5.6-sprint-retrospective}

| *To be completed in Semester 2 as Sprint 3 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

## **7.6 Sprint 4** {#7.6-sprint-4}

### **7.6.1 Sprint Goal and Dates** {#7.6.1-sprint-goal-and-dates}

**Table** 38**:** *Sprint 4 planned goal and dates*

| Sprint goal |  |
| :---- | :---- |
| **Start date** |  |
| **End date** |  |

### **7.6.2 Sprint Planning and Sprint Backlog** {#7.6.2-sprint-planning-and-sprint-backlog}

**Table** 39**:** *Sprint 4 planned backlog*

| Story | Task | Estimate | Owner | Status |
| ----- | ----- | ----- | ----- | ----- |
|  |  |  |  |  |
|  |  |  |  |  |

### **7.6.3 Stand-up and Progress Summary** {#7.6.3-stand-up-and-progress-summary}

| *To be completed in Semester 2 as Sprint 4 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

### **7.6.4 Increment Delivered** {#7.6.4-increment-delivered}

| *To be completed in Semester 2 as Sprint 4 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

### **7.6.5 Sprint Review and Feedback** {#7.6.5-sprint-review-and-feedback}

| *To be completed in Semester 2 as Sprint 4 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

### **7.6.6 Sprint Retrospective** {#7.6.6-sprint-retrospective}

| *To be completed in Semester 2 as Sprint 4 is delivered, using the same structure and tables as Section 7.3.* |
| :---- |

## **7.7 Test Strategy** {#7.7-test-strategy}

### **7.7.1 Testing Approach** {#7.7.1-testing-approach}

| *How the software will be tested in each sprint: unit, integration and system testing, test case design, any test automation, and how acceptance criteria and non-functional requirements will be verified.* |
| :---- |

### **7.7.2 Test Case Template** {#7.7.2-test-case-template}

| *Include a test case template.* |
| :---- |

**Table** 40**:** *Test case template*

| Test ID | User story | Test description | Expected result | Status |
| ----- | ----- | ----- | ----- | ----- |
| TC1 |  |  |  |  |
| TC2 |  |  |  |  |

### **7.7.3 Coding Standards and Traceability** {#7.7.3-coding-standards-and-traceability}

| *State the team’s coding standards, code review and branching rules, and how each requirement will be traced to its test cases.* |
| :---- |

## **7.8 Chapter Summary** {#7.8-chapter-summary}

| *This is a small summary of your chapter.* |
| :---- |

# Chapter 8: Individual Contributions {#chapter-8:-individual-contributions}

## **8.1 Chapter Overview** {#8.1-chapter-overview}

| *This is a small introduction to your chapter.* *CW 1 is a group submission and every team member must contribute to it. Individual contributions will be verified through the evidence listed in Section 8.2 and may be used to adjust individual marks.* |
| :---- |

## **8.2 Verification of Individual Contribution** {#8.2-verification-of-individual-contribution}

| *Individual contribution is verified through the sources below. In the last column, give the link or the evidence reference where each source can be found.* |
| :---- |

**Table** 41**:** *Sources used to verify individual contribution*

| Evidence source | What is checked | Where provided |
| ----- | ----- | ----- |
| **Google Document version history** | Each member’s edits to the portfolio. Any student without Google Document history will be awarded 0 marks. |  |
| **Git commit and pull request history** | Commits and pull requests by each member in the team repository. |  |
| **Task board** | Backlog items and tasks assigned to and completed by each member (e.g. Jira, Trello, GitHub Projects). |  |
| **Supervisor records** | Attendance at the four weekly supervision meetings and their minutes. |  |
| **Team Contribution Record, Individual Contribution Statement and Peer Contribution Estimate** | Agreed by all members (Appendix A and Section 8.3). |  |
| **The viva** | Each member is questioned individually on the portfolio and their own contribution. | Held after submission |

## **8.3 Contribution Summary by Member** {#8.3-contribution-summary-by-member}

| *Summarise the evidence for individual member.* |
| :---- |

## **8.4 Chapter Summary** {#8.4-chapter-summary}

| *This is a small summary of your chapter.* |
| :---- |

# References {#references}

| *Harvard referencing, Westminster style, is the only style accepted.* [*Referencing Your Work: Using Westminster Harvard*](https://www.westminster.ac.uk/sites/default/public-files/general-documents/Referencing%20Your%20Work%20booklet_06.1.pdf) |
| :---- |

# Appendices

| *Add any extra work/materials to this section. You can have multiple sections of the Appendix if needed.* |
| :---- |

**Assessment tips**     

a) In the second year of your degree you should be able to resolve a lot of problems by yourselves. If you do get stuck, look at the later section about ‘managing issues’. Don’t go to your tutor for every question you could find the answer yourself; you are preparing to be independent professionals.  

b) Independent professionals who disappear and no one knows what they are doing, are not professionals and sooner or later get fired. Make sure your tutor knows what you are doing every week (i.e. attend tutorial slots).   

c) You should manage and complete the work as a team. You will have key points where you will show your work to your team-mates to get their feedback. There are more marks for a collegiate, helpful, behaviour to others (without doing their work for them\!) There will be marks lost for ignoring your team-mates, working in isolation, being late with your work, and so on.   

d) Identifying team issues early and managing them is an important part of the module. Minutes of meetings and agreements must also be updated online regularly for your tutor (tutor) to see but also as a record for the team of what you have discussed and agreed.

**Managing issues**  

All work, however well planned, can encounter something unexpected. It is important that you see such issues as learning opportunities and that you manage them, from beginning to end, professionally.   

To resolve an issue yourself:  

a) Do you have all the information about the problem? If not, try to find out the full story.  

b) Could you do something differently yourself and solve the issue? The success of the project will affect you so it is to your interest to adapt if you can.  

c) If the team needs to do something differently, can you convince the group what to do? How can you convince them that what you want will benefit them?  

Raising a case with your tutor:  

a) Have you exhausted the steps for resolving it yourself?  

b) Plan ahead what you want to ask and what you want from them (guidance? action? decision?).   

c) Be respectful of your tutor’s time. Your access to them is during the tutorial slot and only very exceptionally and if it is urgent by email.  

d) Be respectful to your colleagues. All resources are shared and limited, and that includes your manager/tutor. Ensure you are not asking for so much time that others will have to get little or nothing. (It’s actually unprofessional.)  

e) Separate private issues (e.g. “I have a doctor’s appointment next week” is something you should ask to discuss privately), from professional issues (“I'm not clear on how to do this”).  

f) Most of the times your tutor will not solve your problem but will try instead to help you solve it yourself, so you know how to do this in the future.  

Raising a case with your module leader:  

1) Any communication to the module leader must show that it has exhausted all avenues of resolving the issue yourself or with your tutor.

**What do you need to do to get a good mark?**  

Read this document carefully. Manage your work so that you do, typically, another 10 hours of work per week, outside lectures and tutorials. Go to lectures and go to tutorials as you can’t get anywhere else the help and information you need to do well. Seek feedback from your tutor and your teammates. Use that feedback to improve your work. Don’t miss what is on blackboard. Log on blackboard blog what you are doing. Polish your work: document well, write clearly, pay attention to the little details.  Always leave enough time to look at your work again and fix any missed errors.   

**What do you need to do to get a bad mark?**  

Read this quickly and expect someone else will tell you what you missed. Only do a couple of hours of work a week on this module. Don’t come to lectures expecting that you will pick things up from others or from blackboard. Write badly and submit work you did the night before the deadline. Ignore your team mates and their feedback – & give them low quality feedback in return. Assume that you can copy from someone else. Assume that the answer can be found on the internet (it cannot). Miss tutorials and the opportunity to get useful feedback from your tutor. Leave work for the last minute. Come to the presentation unprepared. Think that this is an easy coursework (it is not).  

**Managing issues**  

All work, however well planned, can encounter something unexpected. It is important that you see such issues as learning opportunities and that you manage them, from beginning to end, professionally.   

**Regulations**  

**Assessment regulations**  

Refer to part 3 of the Academic Regulations for a clarification of how you are assessed, penalties and late submissions, what constitutes plagiarism, etc.  

**Penalty for Late Submission**  

If students submit coursework late but within 24 hours of the published deadline, the work will be marked and will have ten percentage points of the overall available marks 

deducted, to a minimum of the pass mark (40% at undergraduate level). If students submit coursework more than 24 hours after the specified deadline, a mark of zero will be awarded for the work in question – unless a claim of Mitigating Circumstances has been submitted and accepted as valid.   

For more detailed information regarding University Assessment Regulations, please refer to the following website: [http\://www\.westminster.ac.uk/study/current-students/resources/academic-regulations](http://www.westminster.ac.uk/study/current-students/resources/academic-regulations%20%20)  

**Finally…**  There is nothing saying that you cannot do very well in this module. You all start with an equal chance to do very well, regardless of how you did last year. But how well you do is up to you and how professionally you are engaging with all aspects of the module. There is a lot of learning to be done with very interesting stuff directly related to how you survive in your future employment. Take it very seriously, but also try to enjoy it.  hel

[image1]: <data:image/png;base64,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>

[image2]: <data:image/png;base64,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>

[image3]: <data:image/png;base64,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+l/9+/S/XA9XI/xYwNvmM/s+37YamuXw9ncXvTxt7pN3mRuPL3/1qSWzHg07FKy5mjPXtdUc/mDpLGgu+EUkOBNc3g//+dIXH77p0duvWD3vuVuv+tm0237/xc719pZzC156JOLXdHtU7Q4FZ6qtP7YLLn649oK2Zmi3bavn33XdLyl91RefrK49shkxzRlKi9i6U/ve8AqvCxceHVFcAoLRw9AUF4XrULvtvTenw6D2+l//xyN/vsIJPcfGt/XVh21NJ++55lf3Xvere6755WO3X/HOnGkw7IDb/MfvuLLq8628qcGvPudoOp6k21DA/MHCF56557q5j98JfRDI8JHtK22K44qTO2c+cstfrvvFU3df/cma+atee2b3hsWgUpqKfdtXvIY4HY3HuD3COqa+DiKvuDB0eG7qtbrKQwnGeHLX+v2b3qk78vHeD5YmWRNU0XJ6j+b8gcp9G1G3W3Xq025n88yHbkr68ATyoY3vXPbDb7047Yagvd6pOl135JPZD90srAsbguKidrPii20wgln52pPznp3a4VAveuHxvR8s05w7cseV//3UHVdPve5Xeze8de3Pv8m0nYGeEQ4KekZnyym/riItzBDwhqpHb7n09SfvBsGo2r+p19kScal++E9TYORUceADkBPGUB20ND1733Ufr34dpCXOtGkr9yvO7UVJq/LY4n4VF9yDG5TaY+9mPJU7Vrx+429+/Mxfbph+z02NX+xpOb0fCgnZGmF8v+ilBz9aNtumPLXwxQdqDm76cMGzYXM1o6/94uM11sYTDuVpcDjNGl564IbLf/C1j5bO1J7b2+PTmuq+2LrqdbgAQDNcrecMNUeqD2/rcLRsmD8dhc2zH74xwerP7f+wrfrgZxsWnN+/UXlqV+u5PS7V6beevXfP6nmC4n4sHeMWK27MVR11NZ7csWLGfdf/6bf/ufuDJavemD7t1stWzHkk4m5e9coTlK6aNdTBua4/ugOFrO3WRvDtup//6y++/T83L3ul9vD2TUtnP3HH1ShoA0Gi2irNDUen33tt04lP4Oq66+qfL3zhoS5X6/l9H4btTR71WbiluP+GX+/btGRIihtzKVyqk4/efhU4Of3Wy5tP7Nyx6jW44Ti96z1386n5M6Ye2PwO6nTMeeTPnL46E7CmOLPixKdHtr27ccmsz9Yv1VUeeXP6A1tXvLnm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>