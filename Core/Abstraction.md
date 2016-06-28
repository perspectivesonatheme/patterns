{Concepts, conception}
- this note deals with conceptual abstraction; need to normalize with [outsourcing](Outsourcing.md) and [integration](Integration.md)

Objects that represent patterns found among phenomena.  
Commonalities as entities distinct from the instances in which they're found.

Abstraction involves inducing a general pattern from specific instances, storing that general pattern as its own concept, and only storing whatever details differentiate specific instances from that pattern on a per instance basis.  Contrast this with storing each instance as a whole.  Not only does this use more bits, but it hides the general pattern behind a layer of obfuscation, making it more difficult to learn about the pattern in order to, for example, predict the behavior of new instances.

Pattern: similarity among phenomena
- a pattern is implicit in its instances; an abstraction is an explicit object representing a pattern
- patterns are of the phenomena; abstractions are of the observer about the patterns
- abstractions only exist in the map, not the territory
	- you could say that the concept TREE exists not only in our minds, but also in DNA; but even there, there's no single piece of DNA that corresponds to TREE; you still have to abstract over all the different physical strands of DNA to realize TREE

Embodiment of abstractions:
- software libraries
	- there can be multiple implementations of a single abstraction (e.g. promises/futures)
- words
	- "cat", "Katze", "猫" as compared to the concept CAT
	- "what's in a name"

Value of abstractions {TODO: simplify}:
- compression
	- efficiency of storage, communication, computation
	- others?
- being able to apply what's learned in one domain to another (analogies)
	- reduces duplication of work
	- less surface area for bugs, including faulty reasoning or unawareness of an aspect of a pattern that was only noticed in a different domain
	- gives you knowledge about unobserved instances
- similar to above: to aid discovery
	- it takes work to find/create efficient abstractions
	- it's much easier to verify an existing abstraction than to find/create one, or even know that one exists to find or would be useful to create ([trapdoor](Search.md#trapdoor))
	- [priming](Priming.md): learning about a pattern/abstraction can help one more easily recognize it
- also similar: abstractions give you a shortcut to the optimal solution
	- if you have a function, you can just plug in the numbers and evaluate; if you don't have a function, you need to guess and check
	- example of determining how much to slow down/speed up clocks on GPS satellites with/without knowledge of relativity
	- analogy of analytical vs numerical math
	- abstractions allow you to solve the problem in an isomorphic {symbolic, virtual} space (e.g. design-space, math-space, cognitive-space) then project the solution back to the implementation-space
	- functors (fmap :: (a -> b) -> f a -> f b, where (a -> b) is the function in the symbolic space)
- inter-system coordination {interfaces}
	- e.g. data interchange formats like JSON and XML allow software systems, by coordinating their behavior, to easily share data
	- or the shared context (set of abstractions) we use to be able to communicate with symbolic language
		- my CAT is the same as your CAT, which allows us to talk about CAT
	- or how monads allow monadic types to be composed in a uniform way (with Haskell's `bind`, which allows things like do notation)
	- all the consensus stuff like electrical outlet plugs, money, etc
	- an interface's specification is an abstraction over the implementations that conform to it
	- {I'm not sure this belongs here; it's more of a use of abstraction rather than a property of it}
- prediction
	- ability to predict the properties and behavior of novel instances (compared to guess and check, observe and recreate {word}, reverse engineer, etc)
	- seems to be a common theme in the above; need to refactor
	- another theme is functors: mapping a category into some isomorphic "virtual" category, performing an operation there, then mapping the result back to the "real" category

Trivia vs general principles

Induction: building a tree from leaves to root; opposite of deduction
- ostensive definition
- the problem of induction
	- Nelson Goodman's new riddle of induction ([occam's razor](Occam's razor.md))
- hasty generalization vs slothful induction
	- quenching and annealing

Science = induction; engineering/design/technology = deduction
- territory -> map vs map -> territory
- science is about decomposing systems into their abstractions
- engineering is about composing abstractions into systems
- [The difference between science and engineering](Http://jadagul.tumblr.com/post/123631186748/ive-decided-lately-that-people-regularly-get)

Chunking: it's easier to remember things that can be chunked using preexisting, general (as compared to ad hoc) abstractions.

Identity: objects are abstractions over patterns in spacetime.

Compression and information entropy.

Examples:
- Football is its own general concept.  The rules don't change from game to game, or if they do, it's easier to store the differences (e.g. college vs NFL or rule changes from year to year) than to store completely separate versions of the sport for each game.
- the concept of proxies (or any of the other patterns, including abstraction itself!)
- knowledge, memory: we store abstract concepts, with specializations built on top of them (e.g. the abstract concept "bird", upon which "bald eagle" is built) (refinement types, genus–differentia definition)
- big words vs a composition of small words (precise vs imprecise, uncommon vs common)
	- big words aid the discovery of concepts, in addition to being more compressed than many small words
	- giving something a name allows you to more easily talk about it; names provide ease of reference
	- names in general
	- big words vs idioms
- freedom of speech: a general principle that is embodied in various laws, which themselves are embodied in the actual enforcement of those laws
- education standards at the local, state, and federal levels (increasing levels of abstraction from the act of teaching)

Anything to say about abstraction to the limit, as discussed [here](Http://www.yesodweb.com/blog/2015/10/beginner-friendly-code-and-apis)?

[levels](Levels.md)  
[emergence](Emergence.md): why do abstractions exist?


### Factorization
The construction of a set of orthogonal (composable/non-redundant/modular/etc) abstractions (a basis) that efficiently spans a subspace.

These bases can be constructed at different levels of abstraction.  With the exception of systems like mathematics (and maybe physics), there most likely doesn't exist (or it wouldn't be practical to construct) a set of abstractions that are perfectly orthogonal and span the entire subspace.  If that's the case, the level of abstraction can be varied to optimize the orthogonality and span of the abstraction set.
- non-ideal abstractions as a result of inaccurate or imprecise factorization; esp. if the basis doesn't have enough dimensions to efficiently factorize the system

Assuming physicalism {naturalism?} is true, everything can be fully explained by (precise enough) physical laws.  However, these laws are too low-level to be of practical use for high-level phenomena.  Therefore, higher-level, emergent laws must be sought, but are rarely found with orthogonality and span to the degree of the physical laws.  These higher-level laws are studied by other sciences, such as chemistry, biology, and sociology. ([emergence](Emergence.md))

{TODO: normalize with [framing](Framing.md)}

"Combing the hairball"  
"Untying the knot"

Normalization

Aspects:
- decomposition of an aggregate into simple parts
- abstraction over simple parts between instances

Factorization within a system vs factorization between systems.  For example, when doing text compression, analyzing just the document of interest vs analyzing general usage of e.g. the English language.
- "within a system" is typically easier because the scope of the content is smaller
- "between systems" has the benefit of using a single basis between systems, which can reduce duplication between individual systems' bases and result in an economy of scale

A power series as an infinite basis where each subsequent term "fine-tunes" the previous ones.  Another infinite basis is the set of primes as factors of the natural numbers.

Refactoring: translating a system into a new basis

Examples:
- the component system for Atmosphere (unreleased video game)
- language design (programming or other)
- this mental framework
- using RGB, HSL, etc to display the color space
- flavor notes?
- axiomatic systems
- factor analysis

[framing](Framing.md)


### Specialization
The optimization of an abstraction for a specific case.

Narrowing {contracting} the scope of an abstraction.  
"Tightness" of an abstraction: how closely the abstraction fits its members  
Refinement

Compared to "all under the same roof", "one size fits all"

Examples:
- hiking with hiking boots vs general-purpose shoes
- engineering: taking general scientific laws and applying them to specific situations
- optimizing an algorithm for a specific CPU architecture
- hardware vs touchscreen keyboard
- handedness?
- "hardware" book vs ebook
	- this also shows the flip side of specialization: by abstracting over books, dictionaries, bookmarks, etc, ebooks have the benefit of integrating cohesive parts of the reading activity
	- more generally, print vs digital display
- musical instrument vs midi keyboard + sound library
- "selective assembly": for the iPhone 5, Apple selectively matches each inlay and housing based on individual fit (see the iPhone 5 design video)

[overfitting](Overfitting.md)  
[overspecialization](Diversity.md#overspecialization)  
[consensus](Diversity.md#consensus): consensus is a reduction of uncertainty which "clears the path" for specialization


### Generalization
Expanding the scope of an abstraction.

When dealing with imperfect {impure, non-ideal} abstractions, there will be a mismatch between the abstraction's intension and each of its instances.  Expanding the abstraction's intension to encompass novel instances decreases precision and increases mismatch, but allows for greater abstraction.  Past a certain point, this mismatch cost may outweigh the benefits of abstraction.

Examples:
- lossy compression (e.g. for music) decreases file size at the expense of quality
