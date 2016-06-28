{TODO: normalize with [abstraction](Abstraction.md) and [outsourcing](Outsourcing.md)}
- see [abstraction-integration](Abstraction-integration.md) for the tradeoffs between abstraction/outsourcing and integration

When a high degree of consensus is reached around a particular system configuration, inter-component costs can outweigh the benefit of modular parts, leading to a monolithic system.  Inversely, a change in requirements (with a corresponding decrease in consensus) can cause the system to move back towards modular parts.  Same thing with an increase/decrease in inter-component costs causing a move towards/away from a monolithic system.

For example, discrete audio components all take up physical space and require being hooked together with cables.  However, when they are integrated into a receiver, these costs are less than the sum of the individual costs—i.e. a receiver takes up less physical space (physical volume, cabinet space, etc) and requires less cabling than the sum of all the discrete components it replaces.  Integrating the parts allows for both an economy of scale (e.g. physical space) and a reduction of inter-component costs (e.g. cabling).  On the other hand, by tightly coupling the components, they can no longer be shared between systems or mix-and-matched with alternative components.  Additionly, because the receiver's components end up sharing parts like the case and power supply, these parts need to be general enough to meet the requirements of all the components instead of being specialized (and therefore, optimized) for any one in particular.
- (Alternative example) Game consoles' CPUs and GPUs can share memory because they're an integrated unit.  By contrast, a PC with equivalent specs can't easily do this because the GPU is interchangeable, so the GPU has to bring its own memory.

It's easier to verify the correctness of a system than to create the system yourself ([trapdoor](Search.md#trapdoor)).  For example, buying an integrated receiver vs building your own and ensuring that all the parts work well together.  A schematic abstracts out the design; a receiver abstracts out the design and construction.

Integrated systems can be inefficient if their parts are general and can be used in many different types of systems.  Integration requires these parts to be duplicated across systems.

Integrated vs abstracted is a relative distinction.  A software library is modular when compared to a program, but integrated when compared to the library's individual functions.

Consolidation

Logistics: the task of coordinating the elements of a complex system

"Batteries included"  
"Everything but the kitchen sink" (implies over-consolidation)

Disjoint: the state of being outsourced when it would be more efficient to be integrated.
- Lack of integration after a consensus has been reached.
- [fragmentation](Diversity.md#fragmentation)

Examples:
- A/V receiver vs discrete A/V components (amp, preamp, DAC, etc)
- IDE vs vim + plugins + unix tools
- framework vs set of libraries
- Mathematica vs Python + NumPy, SciPy, etc
- touchscreen vs hardware keyboard
	- tradeoffs of integrating the keyboard into the screen: can reuse keyboard area for non-keyboard uses, but means that the keyboard must work within the contraints of the screen instead of being specialized for its purpose
- iMac
- Swiss army knife
- smartphone vs mobile telephone + camera + gps receiver + mobile hotspot + portable music player + notepad + flashlight + calculator + clock
- standalone camera vs smartphone + higher quality camera add-on
- iPhone vs Google Ara
- phone batteries: integrated -> removable, specialized (i.e. can only be used with a specific phone model) -> standardized (e.g. AA, external USB)
- end-user maintainability: progression from standardized parts (easy to fix) to integrated wholes (hard to fix)
	- cars, appliances, computers, electronics
- game consoles vs gaming PCs
- AOL vs world wide web
- fish vs zsh
- the centralization of supply chains in large Chinese cities
	- minimizes cost of sourcing inputs because of geographical proximity
- emacs vs vim
	- emacs has broader capabilities while vim is focused on text editing
- Catholicism vs Buddhism
- concentrated animal feeding operations vs family farms
- books vs blog posts vs tweets
	- books need to have more content to offset their higher fixed costs
- waterfall vs agile software development
	- a large release is an integration of multiple smaller releases
	- as the fixed costs of releasing versions decreased (with the web and digital distribution in general), it became beneficial to break up releases into smaller chunks
- cities vs small towns
- US federal vs state government
- European Union
- government vs consumer, labor, etc unions
- brands: "integrating" multiple products under a single label
	- Trader Joe's: integrating brand and store
- Photoshop has functionality for both photos and design/drawing/painting
- leadership {word?}: knowledge is more easily integrated by a single person than across people (given the standard integration vs outsourcing tradeoffs)
- holism vs reductionism
- Apple's software, hardware, and services integration ("walled garden")
- general purpose language vs multiple domain languages
- complex organism vs society of simple organisms
	- human vs ant colony
- department stores vs malls vs standalone speciality stores
- Haskell's stackage: integration of package versions
- databases (generally, global data stores)? esp. as compared to the data model of interacting objects which encapsulate their own data
- pre-made food vs ingredients
- bsd vs gnu/linux
- large nuclear reactors vs small modular reactors
- wikipedia: centralized, has overarching guidelines, format, etc
- vertical integration vs outsourcing
- computer application bloat vs data integration costs
- laptop I/O: integrated ports vs external dock
- "buy local" vs mass production (along the dimension of consumer–producer integration)
	- the "inter-component" costs of mass production include things like difficulty getting information about how something is made or what it's made of
- mass production vs craft production (along the dimension of producer–producer integration)
	- abstraction of design and manufacture (economy of scale)
	- hobbyist/maker -> multinational corporation (e.g. PC industry, 3D printing)
	- beer
		- also shows the reverse trend where diverse preferences provide a pressure back towards craft ([specialization](Abstraction.md#specialization))
- game engine vs render system + game object system + resource system, etc

[diversity](Diversity.md)  
[abstraction](Abstraction.md)  
[critical mass](Criticality.md#critical-mass): of features, etc., before system is worth the fixed costs


### Multiscalar systems
A way to integrate while remaining flexible.  Glue together low level functionality to create higher level functionality.  Give users access to all levels.  Common use cases will use higher levels, uncommon use cases will use lower levels (similar to entropy encoding and compression).  This is only feasible when both the high level and low level functionality can be supported in parallel.

Examples:
- git
- software GUI vs scripting
- smartphones: integrated hardware vs add-on accessories (camera, microphone, etc)

[emergence](Emergence.md): abstractions emerge at various levels
