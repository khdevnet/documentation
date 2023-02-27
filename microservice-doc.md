# Goals
Our system handle business flows with customer,
service responsible for creating/register of a new customer

# Architectural Overview
Note: image could be imported to draw io 
![image](https://user-images.githubusercontent.com/14298158/221689770-c590cace-0ad8-4961-97b6-ce1b285560c7.png)

## Architecture decisions
### Generate Ids for not-verified accounts
System creates only verified accounts and saves them in DB. 
Not verified account temporary created in Redis for 30 minites.
When the customer starts phone verification, system send event to analytics external system. 
System reuse same id created during first attempt of registration, and reuse for other attempts, phone number use to identify user, generated keys saved to Keys table.

### Create new customer
![image](https://user-images.githubusercontent.com/14298158/221689319-daa50268-e5e7-4dbe-8fca-58701c9c499a.png)

## Build and Release Pipelines

* [Build]()
* [Release]()

## Code Repository
* [main]()

## General requirements
* It is a standalone application hosted independently
* It should be market agnostic
* It uses OAuth Authentication, Identity Server as token provider
* The infrastructure deploys using a release pipeline

## Solution requirements
The component is built using .NET 6 using the C# programming language. 
The following [coding guidelines]() are used.

The Layered Architecture Approach was chosen to implement all the required use cases and make components scalable, maintainable, and testable.
* [Solution project guidelines]()

# Quality Assurance Testing
## Environments
### HTTP 
[swagger dev]()   
[swagger uat]()   

### Messages topics/events
[Install-Azure-service-bus-client]()    
[Connect-to-service-bus-and-get-messages]()   

Consumes: customerverified    
Produces: customercreated

### Databases
[Azure MsSQL datbases ]()   
customer-db

## Manual testing
[Microservice-manual-testing-guidelines]()

## Automation testing
We cover by test using [Microservice tests guidlines]()

### Unit tests
All classes should be covered using Unit tests.
You can find tests code styles in the [Unit Tests practices]() guidelines

### Component Tests
Runs using docker container ms sql database.
Runs using wiremock .net 
We cover all API calls using tests.
