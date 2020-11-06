# Duis - online banking for all!
## What is this all about?
Duis is online banking for everyone. The word <b>duis</b> comes from latin and means banking.

This reference architecture demonstrates software development techniques such as Event Storming, CQRS, Event Sourcing, and Domain-Driven Design (DDD) concepts. It is meant as a guide and example on how a software solution can be development from the very first idea to its full implementation. It is important to note that the business domain of banking is explored first from a business perspective and then demonstrate how business concepts and knowledge can be captured on the implemention side. The intention is also to capture the human aspects of it such as communicating with the domain experts. Since banking is a very complex domain, domain-driven design can help capture the complexity of this domain and improve in the quality of the implentation.

The implementation is accomplished using modern tools and services such as the high-performance .net core runtime coupled with the latest AWS serverless technologies. A critical design goal of the solution architecture is to take full advantage of automation and 100% managed services (AWS services). The solution architecture must provide the business with a list of capabilities to stay very competitive but a have extreamly low cost in operation and maintance. It must also be extensible and business capabilities surely will increase over time in part driven by market demands and processes.

## Business Capabilities
As with any software project and unless you have free money to give away, there must be a business driver to accept the fact that it will cost time and money to create a software solution. Let's talk about this for a little. In a typical software project, the budget to <b>create</b> this software accounts for only 10% of the total budget until the software is retired. That means 90% will be spent to maintain the solution over time over meany years once it is in production. It does not matter how small or large the software solution is. Should we not spent a good amount of time understanding the business domain to increase the chances of success? We should also take care that the software is maintainable. We should also design certain parts of the architecture to be replaceable and not put so much emphasis on reusability. Tale a look at the [sacrificial architecure by Martin Fowler](https://martinfowler.com/bliki/SacrificialArchitecture.html).

### Features
Since this is a reference architecture that can certainly be extended with additional features over time, here are the intital sets of business capabilities:

  * Great customer onboarding experience
  * Onboarding of customers, accounts, and their relationships
  * Real-time processing of information as it happens
  * Identifying and triggering of red flags and take action as they happen
  * Guaranteeing 100% correct audit logs as the system records every change for accurate traceability
  * Role based authorizations
  * Generate projections and other reports that include past business events
  * Time travel - easily add new reports and projections as they would have existed at any time in the past
  * Debit and Credit Transactions
  * Automatic fraud detection during onboarding and transaction processing

### Great customer onboarding experience
When new customers onboard with Duis, the experience should be a very smooth one. This means that the user interfaces provided either via mobile apps, web browser, and even native desktop apps must be extreamly responsive. Customers should never have to wait for any kind of response back from Duis. The user interface must capture the customer's intend via clearly marked actions on the UI. It is those actions that will trigger changes to happen on Duis' backend services. Great care should be taken on the look and feel of every UI element including down to pixel perfect positioning. The design for the look & feel of the UI must match Duis' slogan, colors, and overal marketing. 

## Technical Capabilities

