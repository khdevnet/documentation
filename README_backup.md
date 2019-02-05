# Documentation
## Introduction to Technical Writing
### Why technical writing is important
* Marketing: you have to sell you product
* Gets information out of your head: people will stop asking you for it
* Gets the team "On the same page"
* Reduce support calls: (User manuals)
* An auditor might want to know (decisions, solutions)
* It's a direct reflection of you (you should write documentation for people not for you)

### Agile documentation tips
#### (you have to write documentation but not detail)
* Essential (Document with just barely good enough detail)
* Valuable (The benefit of having documentation must outweight the cost of creating and maintaining it)
* Timely (Documentation should be done in just-in-time manner, when we need it)

### Common Technical Documents
* Case studies
* Description
* Emails
* Letters
* Instructions and procedures
* Memos
* Press releases
* Proposals
* Resumes and job applications
* Specifications
* Technical reports
* White papers
* Websites

## The writing process
![](https://github.com/khdevnet/documentation/blob/master/src/writing/process.png)
### Plan phase
#### Purpose
* Requirements - Identify what is to be built, and to verify we’re meeting stakeholders’ expectations
* Design/Architecture - Defines how the system will be constructed, describing critical components and how they fit together
* Code/Technical - Enable task completion and understanding
* Test Plans/Test Cases - Define the approach to testing; expose errors or demonstrate correct behavior
* End-User - Enable task completion; provide support and troubleshooting
#### Audience
![](https://github.com/khdevnet/documentation/blob/master/src/writing/writing-styles-by-audience.png)
#### Delivery
* ask questions where this documentation will be use (web sites, documents)
### Research
* Interview Subject matters Experts
* Review Existing Documentation
* Use the Software
### Write
* Organize you content and ideas (chronological, parts of an object, simple to complex, specific to general)
* Write the first draft
* Check (sentence and paragraph structure, grammar, word choice, spelling)
### Review/edit
* Adjust and reorgonize content
* Editing for style
* Editing for grammar and punctuation
* Revise to incorporate test results
* Usability Testing (line by line testing if guideline works)
### Launch
* Handle translation, if applicable
* Bundle up artifacts
* Coordinate with delopment team and other writers to release
* Create a plan for updates
## Writing tips and best practices 
* Accuracy (document, stylistic, technical)
* Clarity (write weel steps with all details, so the people who doesn't know can do through document from first time)
* Be specific (don't use abstract words)
* Use active voice to describe actions (Check screens A and B for errors)
* Be strong. And say what you mean (assume, depends on, shows, illustrates, requires, needs to, uses differed sometimes, unknown)
* Use shorts sentences
* Use images, charts to describe information
* Use Present tense and be consistence.
## Layout and design 
* Typography (Use typography appropriate for the format and intended use; Focus on readability and understandability using size, contrast and bold/italics)
* Design Principles (Alignment creates a visual connection between elements; Center alignment is usually not as strong as right or left;
Elements closer together are perceived to be more related than elements farther apart; Use contrast to make important elements stand out; Whitespace lets a design breathe, and separates groups of information)
* Page Design Elements (Increase the effectiveness of a document through: Table of contents, Revision history, Headers and footers, Lists/bullets, Captions, Glossary)
* Visuals (Keep visuals simple; If explanation is needed, use a caption; Refer to visuals in the text of the document by their figure or table numbers; Place visuals as close as possible to the text where they are discussed; Consider placing detailed or lengthy visuals in an appendix)

# Deliverables
## Requirements
* Business
* Functional
* Non functional
* Interface
### Use story
![](https://github.com/khdevnet/documentation/blob/master/src/writing/user-story.png)
### Use Cases
![](https://github.com/khdevnet/documentation/blob/master/src/writing/use-case.png)

## Software Design Document
### Introduction
* Purpose
* Scope
* Intended audience
* Design goals and rationale
### System Architecture
* High-level overview of functionality and responsibilities of the system
* Describe high-level components and how they work together
* Diagrams, flowcharts, models, scenarios and high-level use cases showing system behavior or structure 
### Detailed System Design
* Describe in detail the functionality and responsibilities for each component of the system
* Use class diagrams and sequence diagrams to show relationships and flows
### Data Design
* Describe data structures, databases and storage units and their relationships
* Entity Relationship Diagram (ERD) to show structure and relationships
### User Interface
* Describe functionality from the user's perspective
* Wireframes or mockups of what the UI will look like
* Describe the controls and their behaviors
* Supported orientations and dimensions
### Glossary/Appendix

## Code documentation
### Code comments
* don't use dead code
* don't comment obvious things, use comments to describe not obvious things
* generate documentation from comments if it is portable library or API
* Use "TODO" stataments in code

### API documentation 
* use automate API documentation generators like swagger.io, mashery.com, apiary.io, raml.org, ASP.NET Web API
* describe API in place where all team members can view it

### Readmes
* Date
* Software name and version number
* Short description of the software
* Installation requirements and instructions
* Copyright and licensing information
* Contact information for the developer or distributor
* A file manifest (list of files included)
* Configuration instructions
* Operating instructions
* Known bugs
* Troubleshooting
* Credits and acknowledgments
* Change log (usually for developers)
* News/updates (usually for users)

## Test Plans and Test Cases
### Introduction
#### Purpose
Purpose of the document and short summary of the main sections
#### Project overview
Briefly describe the project and software being tested
#### Intended audience
* Who is the intended audience for the document?
* What is their role in the testing process?
### Test Strategy
#### Test objectives
* What will you test and why?
* What is in scope and out of scope?
* Common test types: Module testing; Integration testing; Acceptance testing; Beta testing
#### Test assumptions
List conditions that must be true in order to be successful in testing
* Realistic test data is available
* Knowledge and skills of testing resources are adequate
#### Test principles
Foundational characteristics of the testing approach and process
* Test processes will be well defined, yet flexible enough to change if needed
* Testing environment and data will match a production environment as closely as possible
* Testing will be divided into phases, each building on the previous
#### Data approach
* Describe the data that will be loaded (or not loaded) for test activities
#### Scope and levels of testing
At a high level, describe the types of testing to be performed, along with the scope and timing of each
* User Acceptance Testing (UAT)
* Validates the business logic
* Performed by end users
* The test team will write tests based on input from the business analyst and end users
* Testing will be performed after all other testing is complete
#### Estimated effort and resources
* List all activities to be performed by the QA team, along with estimated effort hours
### Execution Strategy
#### Entry and exit criteria
Entry criteria: the conditions that must exist in order to start testing    
Example: All test data is loaded into the environment   
Exit criteria: the conditions that must be met to proceed with the next cycle/release   
Example: Pass rate of 95% of test scripts   
#### Test cycles
For each type of testing (e.g., Functional testing, UAT, etc.), describe how many cycles will be executed, along with the objective for each
Example:
* Functional testing will occur in two cycles
* The first cycle is intended to identify critical defects
* The second cycle is intended identify medium and low defects, and to validate correction of defects found in the first cycle
#### Defect management
Describe the approach to identifying and managing defects
* Labeling (e.g., critical, high, medium, etc.)
* Tracking tools (e.g., TFS, JIRA)
* Information required to be documented when opening a defect
* Roles and responsibilities
#### Metrics
Outline metrics to be reported on the project, along with frequency
* Weekly: % complete, % pass, % fail
* Weekly: Status report
* Daily: Critical defects
#### Defect tracking and reporting
Define the process/flow for tracking and reporting defects
### Test Management Process
#### Test management tool
Provide details about the tool(s) used for managing tests (e.g., Excel, TFS)
* Location of tool
* Permissions required
* Reports
#### Test design process
How will tests be designed and written?
Example:
* Tester reviews requirements
* Map test case to requirements in traceability matrix
* Tester and BA create test cases
* SME reviews the test cases and provides sign-off
#### Test execution process
What’s the process for executing tests?
Example:
* Tester executes each step in the test case
* Mark status as Pass or Fail
* Raise defects as needed
* Participate in Triage meetings to help route defects as appropriate
#### Test risks and mitigation factors
Call out risks and mitigation plans
* Resources (people and money)
* Schedule
* Scope
* Defects
#### Communications plan
How will communication happen on the project and who should be involved?
* Meetings
* Emails
* Status reports
* In-tool communications
#### Roles
Identify roles on the project, along with the name and contact information of the person filling that role
* Project manager
* QA lead
* QA team
* Business analyst
* Development lead
* Development team
* Other stakeholders
### Test Environment
* Location of software to be tested
* Permissions
* Hardware and software required for testers
* Contact information for support

## Test scenario
![](https://github.com/khdevnet/documentation/blob/master/src/writing/test-scenario.png)
## Test Case
* Anyone can execute it
* All necessary details are included
* Strong, descriptive title
* Consistent naming conventions
* Legible and easy to understand
![](https://github.com/khdevnet/documentation/blob/master/src/writing/test-case.png)
* Reusable

## End-User Documentation
### User Guides
#### Overview
* High-level description of the product
* Major features
* Benefits
* How it fits with other products
#### Getting Started
* Setup and configuration information
* Prerequisites for using the system
* Task-based so that the user can start using the system quickly
#### Tutorials
* Organized by main features or tasks
#### Troubleshooting
* Detail possible errors or problems and describe how to resolve them
#### Frequently Asked Questions (FAQs)
* Common questions that user have, along with answers and references to additional information
#### Support
* How to get additional help
* Contact information
#### Glossary
#### Index
### Quick Reference Guides
* Diagrams
* Reference tables
* Steps
* Graphics/infographics
### Release Notes
Documents the differences between two versions of the same software (e.g., v1and v2)
#### Release date
#### Product version
#### Previous product version
#### New Features
* List any net new features or functionality in this release
* What are the benefits of the new feature?
#### Known Issues
* List any bugs that are known to exist when the software releases
#### Enhancements
* List changes to existing features
* What is the justification for the change?
* How is the change beneficial?
#### Resolved Issues
* Detail any problems that existed in the previous release that were fixed in this release
* Include the solution to the issue
#### Frequently Asked Questions (FAQs)
* Common or anticipated user questions and their answers
#### Optional (usually only if changed since previous release)
* System requirements
* Installation instructions
