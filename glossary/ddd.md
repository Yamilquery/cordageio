## Domain Drive Design Glossary

|Concept|Context|Description|
|--|--|--|
|Event Sourcing|DDD|Capture all changes to an application state as a sequence of events. Layered architecture that is almost always inspired by a CQRS design that focuses its logic on events rather than plain data. Events are treated as first-class data, and any other queryable information is inferred from stored events.|
|Domain Model|DDD|Layered architecture based on a presentation layer, an application layer, a domain layer, and an infrastructure layer, designed in accordance with the DDD development style. In particular, the model is expected to be a special type of object model.|
|Client/server architecture|DDD|Classic two-layer (or two-tier) architecture that consists only of presentation plus data access.|
|Multitier architecture|DDD|Segmentation that is in many ways similar to that of a multilayer architecture except that now multiple tiers are involved instead of layers. (More on the possible downsides of a layer-to-tier mapping in a moment.)|
|Multilayer architecture|DDD|Canonical segmentation based on presentation, business, and data layers. The architecture might come in slightly different flavors, such as an additional application layer between the presentation and business layers and with the business layer transformed into a domain layer by the use of a DDD development style. Layered architecture is just another name for a multilayer architecture. We’ll be using the term layered architecture instead of multilayer in the rest of this chapter and throughout the book.|
|Monolithic architecture|DDD|The context is a standalone application or service that exposes an API to the rest of the world. Typical examples are autonomous web services (for example, Web API host) and Windows services. Yet another example is an application hosting a SignalR engine.|
