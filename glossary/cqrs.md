## Glossary Command Query Response Seggregation CQRS
|Concept|Context|Description|
|--|--|--|
|Aggregate|CQRS|A larger unit of encapsulation than just a class. Every transaction is scoped to a single aggregate. The lifetimes of the components of an aggregate are bounded by the lifetime of the entire aggregate. Concretely, an aggregate will handle commands, apply events, and have a state model encapsulated within it that allows it to implement the required command validation, thus upholding the invariants (business rules) of the aggregate.|
|Aggregate Root|CQRS|The aggregate forms a tree or graph of object relations. The aggregate root is the "top" one, which speaks for the whole and may delegates down to the rest. It is important because it is the one that the rest of the world communicates with.|
|Command|CQRS|Commands are things that indicate **requests** to our domain. While an event states that something certainly happened, a command may be **accepted** or **rejected**. An accepted command leads to zero or more events being emitted to incorporate new facts into the system. A rejected command leads to some kind of exception.|
|Projections|CQRS|is a read-only view of some application state, built up from the published domain events.|
|Projectors|CQRS|A projection is built by a projector module defined as an event handler: it receives each published domain event and updates the read model. So a projection is read model state that is projected from domain events by a projector.|
|Queries|CQRS|is a request for data or information from a database.|
|Anticorruption layer|CQRS|Indicates an extra layer of code that hides to the downstream context any changes implemented at some point in the upstream context.|
|Shared kernel|CQRS|Two contexts share a subset of the model. Contexts are therefore tightly coupled, and no team can change the shared kernel without synchronizing with the other team.|
|Validators|CQRS|It serve to create validation rules for the current context. For example, unique email validation|
|Support Middlewares|CQRS|is an the extension point to include cross-cutting concerns into command dispatch. This can be used to add in command validation, authorization, logging, and other behaviour that you want to be called for every command the router dispatches. You define your own middleware modules and register them in your command router. They are executed before, and after success or failure, of every dispatched command.|
|Support Validators|CQRS|Here are all the common validation rules to execute during the execution of commands. For instance, UUID parse validation|
