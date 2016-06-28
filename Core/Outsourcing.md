{TODO: normalize with [abstraction](Abstraction.md) and [integration](Integration.md)}
- see [abstraction-integration](Abstraction-integration.md) for the tradeoffs between abstraction/outsourcing and integration

Putting an interface between entities allows them to vary independently, as long as they both conform to the interface's specification.

The abstraction of objects or processes. {?}

"Civilization advances by extending the number of important operations which we can perform without thinking about them." (Alfred North Whitehead)

No single person knows how to make a pencil.
- all of the parts to a standard pencil are outsourced to specialized producers

Reductionism: efficient outsourcing relies on the ablility to decompose a system around simple interfaces.

Modularity {composability, abstraction, destructuring}

Examples:
- food, clothing, shelter
- cleaning, child care
- outsourcing parts of thought and communication to specialized languages (e.g. math)
- beliefs: outsourcing beliefs to other people or organizations
- mental abilities
	- outsourcing memory to notes, books, Google
	- calculators, computers in general
- skills
	- Basic skills like arithmetic don't need to be known to a high level of proficiency (e.g. doing complex mental math) because arithmetic can be outsourced to computers.
	- Similarly, a programmer's need for proficiency in writing assembly code decreases as compilers' abilities in translating high-level languages to assembly increases.
	- The mean of this distribution moves toward more and more advanced (and hence specialized) skills/knowledge as more and more skills/knowledge become commoditized.
- consultants, contractors and subcontractors
- in contrast to homemade
- microservices
- outsourcing code to a function (or library)
	- and the opposite is inlining, necessary because of the costs of the function interface
- outsourcing to team members (delegation)
- the unix philosophy

[interfaces](Interfaces.md): e.g. between producers and suppliers (e.g. specifications)  
[diversity](Diversity.md)


### Parallelization
Parallelization requires the parallelized to be outsourced.

If part of a system needs to be dynamically (horizontally) scalable, that part requires an interface.

Relationship to reductionism: e.g. parallel computations can't be dependent on one another

Interface costs: e.g. swappable battery mechanism, overhead from threading

"Too many cooks in the kitchen"
- tasks can only be split up so much before coordination costs outweigh the benefits of parallelizing work
- diminishing or negative returns from increasing number of threads performing a computation

Examples:
- distributed/parallel computing
- divide and conquer
- swappable batteries
- load balancer between clients and servers
- sourcing from multiple suppliers in order to increase a part's supply
- small modular nuclear reactors
