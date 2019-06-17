Anything that acts as a common interface between sets of disparate entities.

The sets of disparate entities may be factorized of competitive alternatives (sum types? https://en.wikipedia.org/wiki/Tagged_union) and/or cooperative elements (product types?).

The interface must provide the primitives necessary to "host" its users.
- for example, IP can host any arbitrary data format
- users unable to be hosted by the interface may be less viable than if there were no common interface because of the consolidation around the common interface
	- similarity with [controlled defects](Controlled%20defects.md) or [watershed](Watershed.md): the hostable users are helped, the unhostable users are hurt
- the common interface is essentially the least common multiple, or union, of all of its users' specialized interfaces (or the union of all one-to-one interfaces between all of its users)
	- however, because of the costs of [generalization](Abstraction.md#generalization), the common interface may not provide a perfect superset of the specialized interface's functionality

Entities may require an adapter to connect to a general interface (e.g. a cable jack).

"Hourglass shape": many sources, single interface, many sinks

Examples:
- internet protocol
- electricity: multiple sources and uses
- web: html, css, js as the intermediary between server and client
- money: many ways to earn, many ways to spend
- instruction set architecture
- specifications, e.g. for a component of a machine
- APIs
- languages: the shared context (set of abstractions) used to be able to communicate
- [markets](Markets.md) {exchanges}
- producers, as the interface between multiple suppliers and consumers
- contracts
- legos
- food, water, air as interface between an organism and its environment
- standard cables and jacks (as compared to "hard-wired")
- data interchange formats like JSON and XML
- monads allow monadic types to be composed in a uniform way (e.g. Haskell's do notation)
- cell membranes that allow inflow/outflow of chemicals?

[consensus](Diversity.md#consensus): having a single common interface can be more efficient than having multiple custom interfaces  
[media](Media.md)  
[outsourcing](Outsourcing.md): outsourcing requires some sort of interface between the outsourcer and the outsourced
