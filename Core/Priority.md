{precedence}

The ordering of concerns by importance.

When a concern is of primary importance, with other concerns being addressed in a subordinate manner.

{dominant, principal} vs {residual, remainder}  
"Progressive precision"
- axe, hatchet, chisel, sandpaper

Note that priority is usually not cut and dry, e.g. if a goal is impossible due to subordinate concerns. However, this may be caused by a defect in the specification of the concerns. One or more concerns are probably aggregates of smaller, more fundamental concerns, and should be refactored. Nevertheless, such refactoring can often be impractical, necessitating a slightly more global view of the problem rather than a purely local view of the primary concern.

Violation of this pattern often called "the tail that wags the dog". Or "putting the cart before the horse". "You can't shine shit". "Putting lipstick on a pig".

"Smoke test": validating an early property  
"Fine tooth comb": addressing later concerns

Examples:
- software: make it work, then make it beautiful, then make it fast
	- premature optimization
	- beautifying code that doesn't solve the right problem
- establish the utility of the product/idea/etc, and then figure out how to market it
	- alternatively: create something of value, then find the money
- 80-20 rule, Pareto principle: don't waste time fixing little things when there are big things to fix
