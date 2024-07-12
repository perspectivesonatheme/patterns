The variation of alternatives.

Maintaining diversity vs settling on the current best option\
Hedging bets vs optimizing given the current knowledge\
Generalization vs specialization

Creativity is the creation of more diversity.

A note on the word "diversity":
- can be used for both differences among alternatives, but also among elements of a whole (e.g. parts of a machine, roles in a company); this pattern is about the former
- i.e. this is about competition between alternatives, not the synergy of a diverse set

Aspects:
- experimentation: when there is uncertainty about the design of something, diversity allows for the experimentation of different designs to see what works best ([testing](Testing.md))
- diversification {hedging, insurance}: guarding against changes in externalities
	- experimentation regards uncertainty in the optimal design of the system, whereas diversification regards uncertainty in the future state of its environment
	- "Don't put all your eggs in one basket."
	- genetic diversity and extinction events
	- sourcing the same part from multiple suppliers
	- hedging bets

Language:
- collapse: the resolution of diversity, implying prematurity
- resolve {reconcile}: a proper resolution of diversity
- selection pressure: the pressure towards resolution

Examples:
- evolution: genetic diversity from mutations and sexual reproduction
- ideas
- science: multiple theories and experiments attempting to answer a question; compare with religious dogma
- "ways of living life", including diets
- rebellion is a way of increasing diversity by challenging the accepted status quo; essentially spot-checking cultural norms
	- hipsterism and the rejection of popular music
- diversity in languages vs single universal language
- the federal system is intended to maintain diversity by putting some control at the state and local levels, then graduating what works to the federal level
- private industry and government
	- private industry supports competition among diverse approaches, but can be inefficient for industries which lack competition due to consensus, consolidation, or natural monopoly
	- governments tend not to foster diverse approaches, but don't suffer from the same issues as private industry when competition is untenable/unneeded
- cpus, gpus, floating point, game consoles
- brain development: the balance between hardwired, inflexible, fast development, and plastic, adaptable, long period of development
- privacy as a way to prevent a premature collapse of diversity
	- esp. when a belief, way of living, etc is taboo but not wrong
- globalization
- "being opinionated" in software frameworks: collapsing diversity based on the current best practice
- [The Refragmentation (Paul Graham)](http://paulgraham.com/re.html): historical trend of increasing diversity in the US from the mid 1900's forward

One needs to consider the level at which diversity or consensus happens. For example, if a team/machine operates best with a variety of individuals/parts, consensus is only beneficial between similar parts or perhaps between the whole and other wholes, but not between disparate parts. ([outsourcing](Outsourcing.md))

Another distinction to make is between diversity and [parallelization](Outsourcing.md#parallelization). Multiple people or machines of a single organization may have the same role in order to speed up the work or increase bandwidth, but this would not be considered diversity as defined here.

Demand-side diversity {fragmentation}
- in this case, there can be no consensus on the supply side because multiple demands need to be satisfied
- e.g. varying preferences: taste, fashion, etc
- [specialization](Abstraction.md#specialization)

[annealing](Annealing.md): decreasing diversity as uncertainty is decreased?\
[uncertainty](Uncertainty.md): diversity is needed in proportion to the amount of uncertainty\
[traction](Traction.md)\
[facilitation and production](Facilitation%20and%20production.md): combining existing elements in new ways vs creating new elements from scratch\
[emergence](Emergence.md)\
[abstraction-integration](Abstraction-integration.md): need to normalize diversity with abstraction-integration


### Consensus
{consolidation, coordination, coalescence, standardization}

Nucleation: the formation of an initial consensus

A zipper as a physical analogy: consensus is the zipped part, diversity as the unzipped part\
Analogy of a magnet. Normal iron has magnetic spin pointing every which way. But magnetized iron's spins all line up.

Does consensus need to be distinguished from coordination?
- consensus is agreement on what the best thing is
- coordination is everyone picking the same thing
- there can be coordination without consensus and consensus without coordination

It can be beneficial to promote a partial consensus if it aids discovery, standardization, etc, while still allowing alternatives.
- built-in notepads on phones
- standard libraries in programming languages

Examples:
- bitcoin: distributed database that everyone agrees on
- money
- science
- voting
- "eigenmorality": http://www.scottaaronson.com/blog/?p=1820&re=1
- prediction markets
- Wikipedia: knowledge consensus
- single charger type for mobile phones
- electrical outlets (at least within a country)
- the internet: all nodes speak IP
- the web: html, css, js
- culture: people within a culture coordinate their behavior
	- e.g. the US uses the English units measurement system
	- (US) handshaking and hugging are the standard greetings; compared to bowing, saluting, etc
- vhs vs betamax, bluray vs hd-dvd
- ascii and unicode
- Arabic numerals, decimal system
- Atul Gawande - The Checklist Manifesto
- QWERTY
- metric system
- English as a global language
- lingua franca
- shipping containers


### Fragmentation
Diversity beyond the amount prescribed by the level of uncertainty is fragmentation.  Fragmentation implies unnecessary duplication of work and impedes consensus, critical mass, etc.

Examples:
- the digital ecosystems of Google, Apple, Microsoft, Amazon, Facebook; come with large switching costs which inhibit competition
	- may be only a short-term phenomenon
- the variety of ways of sending money between people, none of which are ubiquitous
- "too many cooks in the kitchen"?
	- limited resources (space, equipment) + increasing coordination costs
- vim and emacs: lots of diversity but little consensus; makes it difficult to get set up, more fragmentation in plugins and documentation, etc
	- each plugin has fixed costs, which together can outweigh the cost of lack of diversity due to standardization
	- e.g. for vim, plugin managers: pathogen, vundle, neobundle
	- distributions like spacemacs and spf13 can help, but can also just move the problem one level up if no distribution is de facto, sanctioned, etc
	- but the deeper problem with distributions like those is that they only have so much control, and as such, have limited ability to integrate
- when there's multiple political candidates of similar ideology in an election, splitting the vote (in plurality voting systems)
- each mobile phone manufacturer used to have its own proprietary charger plug
- the US uses both the US customary and metric systems
- web developers had to support old versions of IE separate from standards compliant browsers
- private health insurance vs single payer: duplication of profits and overhead
- instant messaging services
- the English language has inconsistent rules for spelling, pronunciation, etc because it has adapted words from multiple other languages, without integrating them within a single consistent framework
- English second person plural: you, y'all, you guys, you lot, ye
- analysis paralysis

[integration](Integration.md): fragmentation can be caused by both disorder and integration


### Overspecialization
{Overfitting, premature-optimization, collusion, over-precise, over-abstraction?, overgeneralization}

Diversity less than the amount prescribed by uncertainty.
- Overspecialization is not only caused by a premature collapse of diversity, but can also be caused by a change in externalities.  For example, fixed function GPUs were efficient for a time, until increasing transistor budgets and changes in the demands of software reached a point at which general purpose GPUs became favorable.

Can happen when selecting from currently available solutions when none of them meet some standard of acceptability.
- from this perspective, [analysis paralysis](Uncertainty.md#analysis-paralysis) is not always a bad thing ([bias interpretation](Bias%20interpretation.md))
- selecting the least bad solution can lead to churn, where the new solution is found to have many faults, encouraging the selection of a new solution, with the same result if nothing is changed about the decision process or no good solutions have yet been found
	- the rapid churn of web tech

Examples:
- web tech initially being designed for documents
- monocultures, incl. in agriculture
- learning foreign languages can protect against overfitting to a single language
- progression from fixed function to programmable GPUs
	- the "backing out" of specializations made given the constraints of hardware and demands of software
