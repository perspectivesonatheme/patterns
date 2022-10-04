The tradeoffs between abstraction and integration.

This note contains a high level overview.  For examples and more information on the individual patterns, see [abstraction](Abstraction.md), [outsourcing](Outsourcing.md), and [integration](Integration.md).


**Abstraction** {destructuring, outsourcing, modularity}: pulling a part out into its own entity
- *reuse* {deduplication, compression}: sharing of the part across multiple systems
- *specialization*: optimization of the part's design for its specific purpose
	- if the part is integrated, its design is constrained by the rest of the system (e.g. touchscreen vs hardware keyboard; software rendering vs GPU)
<br><br>
- *experimentation* {competition, interchangeability, fungibility}: different part designs can be tested without changing the rest of the system
- *parallelization* {scalability}: parallel usage of arbitrarily many instances of a part (dynamic horizontal scaling)
- *diversification* {redundancy, hedging}: guarding against external risks by supporting a diversity of designs

**Integration** {monolithic systems}: combining a part and the rest of the system into a single entity
- *cohesion* {tight coupling}: reduction of interface costs
- *economy of scale*: sharing of costs between the parts of a system
<br><br>
- *discovery*: it's easier to evaluate the efficiency of a system than to design one from scratch (abstraction of system design)


{TODO: need a unified model for this.  *Reuse* and *economy of scale* are essentially the same thing, as are *specialization* and *cohesion* {maybe}.}

[integration](Integration.md)\
[outsourcing](Outsourcing.md)\
[abstraction](Abstraction.md)
