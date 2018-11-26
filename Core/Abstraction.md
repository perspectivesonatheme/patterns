{Concepts}
- this note deals with conceptual (map–territory) abstraction; need to normalize with [outsourcing](Outsourcing.md) and [integration](Integration.md)

Objects that represent patterns across phenomena.  
Commonalities as entities distinct from the instances in which they're found.  
As a process: inducing a general concept from specific instances.  
Universals

Considering {regarding} one aspect of an object in isolation from others.  
Ignoring irrelevant details {information}.

Pattern: similarity among phenomena
- a pattern is implicit in its instances; an abstraction is an explicit object representing a pattern ([reification](Reification.md))
- patterns are of the phenomena; abstractions are of the observer {word} about the patterns
- abstractions only exist in the map, not the territory
- for example, a repeated chunk of code is a pattern; a function that is called in place of each chunk is an abstraction
- there can be multiple abstractions representing a single pattern; for example, multiple people looking at a repeated chunk of code will each have an abstraction in their minds representing it

Embodiment of abstractions:
- software libraries
	- there can be multiple implementations of a single abstraction (e.g. promises/futures)
- words
	- "cat", "Katze", "猫" as compared to the concept CAT
	- "what's in a name"

Value of abstraction {TODO: refactor}:
- compression
	- efficiency of storage, communication, computation
	- others?
- being able to apply what's learned in one domain to another (analogies)
	- reduces duplication of work
	- less surface area for bugs, including faulty reasoning or unawareness of an aspect of a pattern that was only noticed in a different domain
- similar to above: to aid discovery
	- it takes work to find/create efficient abstractions
	- it's much easier to verify an existing abstraction than to find/create one, or even know that one exists to find or would be useful to create ([trapdoor](Search.md#trapdoor))
	- [priming](Priming.md): learning about a pattern/abstraction can help one more easily recognize it
- also similar: abstractions give you a shortcut to the optimal solution
	- if you have a function, you can just plug in the numbers and evaluate; if you don't have a function, you need to either measure or guess and check
	- example of determining how much to slow down/speed up clocks on GPS satellites with/without knowledge of relativity
	- analogy of analytical vs numerical math
	- abstractions allow you to solve the problem in an isomorphic {symbolic, virtual} space (e.g. design-space, math-space, cognitive-space) then project the solution back to the implementation-space
	- functors (fmap :: (a -> b) -> f a -> f b, where (a -> b) is the function in the symbolic space)
- prediction
	- ability to predict the properties and behavior of novel instances (compared to guess and check, observe and recreate {word}, reverse engineer, etc)
	- seems to be a common theme in the above; need to refactor
	- another theme is functors: mapping a category into some isomorphic "virtual" category, performing an operation there, then mapping the result back to the "real" category
- isolation of an aspect allows full application of computational/brain power to just that aspect instead of being distributed among all aspects of the system

Different "views" of abstraction:
- projection: considering an aspect in isolation
- generalization: commonalities between instances as a single concept
	- relation to projection: objects can be generalized-over when they are "equal under projection"
- encapsulation: defining an object by its specification instead of by its implementation
	- relation to projection: the specification is one aspect of an implementation
	- relation to generalization: many implementations can have the same specification—the specification is the generalization of all conforming implementations

Trivia vs general principles

Induction: building a tree from leaves to root; opposite of deduction
- ostensive definition
- the problem of induction
	- Nelson Goodman's new riddle of induction ([Occam's razor](Occam's%20razor.md))
- hasty generalization vs slothful induction
	- quenching and annealing

Science = induction; engineering/design/technology = deduction
- territory -> map vs map -> territory
- science is about decomposing systems into their abstractions
- engineering is about composing abstractions into systems
- [The difference between science and engineering](http://jadagul.tumblr.com/post/123631186748)

Chunking: it's easier to remember things that can be chunked using preexisting, general (as compared to ad hoc) abstractions.

Identity: physical objects are abstractions over patterns in spacetime.

Compression and information entropy

Superordinate and subordinate

Examples:
- football is its own general concept; the rules don't change from game to game, or if they do, it's easier to store the differences (e.g. college vs NFL or rule changes from year to year) than to store completely separate versions of the sport for each game
- the concept of proxies (or any of the other patterns, including abstraction itself!)
- knowledge, memory: we store abstract concepts, with specializations built on top of them (e.g. the abstract concept "bird", upon which "bald eagle" is built) (refinement types, genus–differentia definition)
- big words vs a composition of small words (precise vs imprecise, uncommon vs common, ad hoc vs composed)
	- big words aid the discovery of concepts
	- big words are usually more compact than an equivalent composition of small words
	- giving something a name allows you to more easily talk about it; names provide ease of reference
	- names in general
	- big words vs idioms
- freedom of speech: a general principle that is embodied in various laws, which themselves are embodied in the actual enforcement of those laws
- education standards at the local, state, and federal levels (increasing levels of abstraction from the act of teaching)
- money: a way of comparing values of otherwise incommensurable things

Anything to say about abstraction to the limit, as discussed [here](http://www.yesodweb.com/blog/2015/10/beginner-friendly-code-and-apis)?

[levels](Levels.md)  
[emergence](Emergence.md): why do abstractions exist?


### Specialization
The optimization of an abstraction for a specific case.

Narrowing {contracting} the scope of an abstraction.  
"Tightness" of an abstraction: how closely the abstraction fits its instances  
Refinement

Compared to "all under the same roof", "one size fits all"

Examples:
- hiking with hiking boots vs general-purpose shoes
- engineering: taking general scientific laws and applying them to specific situations {is this really specialization?}
- optimizing code for a specific CPU architecture
- hardware vs touchscreen keyboard
- handedness?
- paper book vs ebook
	- this also shows the flip side of specialization: by abstracting over books, dictionaries, bookmarks, etc, ebooks have the benefit of integrating cohesive parts of the reading activity
	- more generally, print vs digital display
- musical instrument vs midi keyboard + sound library
- "selective assembly": e.g. the iPhone 5's inlays and housing are selectively matched based on individual fit (see the iPhone 5 design video)
- domain-specific vs general
	- AI, languages

[overfitting](Overfitting.md)  
[overspecialization](Diversity.md#overspecialization)  
[consensus](Diversity.md#consensus): consensus is a reduction of uncertainty which "clears the path" for specialization


### Generalization
Expanding the scope of an abstraction.

When dealing with imperfect {impure, non-ideal} abstractions, there will be a mismatch between the abstraction's intension and each of its instances.  Expanding the abstraction's intension to encompass novel instances decreases precision and increases mismatch, but allows for greater abstraction.  Past a certain point, this mismatch cost may outweigh the benefits of abstraction.

Examples:
- lossy compression (e.g. for music) decreases file size at the expense of quality
- labels, “-isms”
- stereotypes
