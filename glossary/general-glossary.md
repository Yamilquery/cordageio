# Cordage.io

Ubiquitous Language is the term Eric Evans uses in  [Domain Driven Design](https://www.amazon.com/gp/product/0321125215?ie=UTF8&tag=martinfowlerc-20&linkCode=as2&camp=1789&creative=9325&creativeASIN=0321125215)![](https://www.assoc-amazon.com/e/ir?t=martinfowlerc-20&l=as2&o=1&a=0321601912)  for the practice of building up a common, rigorous language between developers and users. This language should be based on the [Domain Model](https://martinfowler.com/eaaCatalog/domainModel.html)  used in the software - hence the need for it to be rigorous, since software doesn't cope well with ambiguity.

Evans makes clear that using the ubiquitous language between in conversations with domain experts is an important part of testing it, and hence the domain model. He also stresses that the language (and model) should evolve as the team's understanding of the domain grows.

## Glossary Contexts

|Context|Description|
|--|--|
|DDD|Domain Driven Design. Set of patterns for building enterprise applications from the domain model out|
|CQRS|[CQRS](https://martinfowler.com/bliki/CQRS.html)Two-fold layered architecture with parallel sections for handling command and query sides. Each section can be architected independently, even with a separate supporting architecture, whether that is DDD or client/server.|
|Sales and Marketing Terms| This is a context that covers terms used in sales, and in marketing at cordage. While these may not appear to have any relevance in the development process.|
|Internal Processes| Internal processes is a catch-all term in which we define the glossary for both agile development and product development.|
|[Rigging](https://github.com/cordageio/rigging/blob/master/docs/ubiquitous/glossary/README.md)|Rigging is a the name given to the context that manages: Organizations, Locations, Teams, Users, and user Security.|
|RBAC|Role Based Access Control is a way to prevent unauthorized access to documents and preferences to limited users. This is a standard functionality in large enterprises. RBAC can be used to facilitate administration of security in large organizations with hundreds of users and thousands of permissions. These are used to enforce these policies without any complication.|
|Frontend|Frontend is the graphical interface that allows a user to view and interact with data. This is also called the interaction layer and is mostly built with HTML, CSS and Javascript (Pure or with tools like React)|
|On-Premise|On-premises (abbreviated as "on-prem" or incorrectly said as "on-premise") is software that is installed and managed by the client organization in their own servers.|
|Billing| Refers to the automated process of sending an invoice/bill to a customer in exchange for goods or services rendered.|
|Logs-reports-notifications|A log, in a computing context, is the automatically produced and time-stamped documentation of events relevant to a particular system. A report is the grouping of log activities to provide value to the end user. A notification is an action triggered by an event registered in the log. At Cordage we grouped these three elements inside a context because they all revolve around the registration of an event.|
