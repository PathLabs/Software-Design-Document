# Module and Interface Descriptions

## Intro
**TODO**

## Module 1
**TODO**

## Module 2: Primer Scoring
The second module planned for the final product describes designing an interface around another step in the pipeline. This step in particular shall take the results of module 1, groups of possible primers, and scores them on a variety of factors. In order to accurately score these primers, the program needs the following inputs:


1. Optimal melting temperature for the reaction
2. Optimal range for GC content
3. Importance scale for each of the following features:
    * Tm: minimize the distance of primers from optimal melting temperature
    * GC: minimize distance of primer GC% out of optimal range
    * Homopolymers: minimize the amount of homopolymer in primer
    * Dimerization: minimize the amount of self dimerization in primer
    * Specificity: minimize the number of times primers appear in background
    * Degenerate: minimize the number of degenerate/ambiguous bases in the primer


In order to provide a working product, the team must provide a usable interface, that provides input elements for each of the aformentioned requirements. According to the design document signed by the client, the interface is designed to look approximately like the following diagram, given some changes based on usability testing:

**TODO: Diagram**

## Module 3
**TODO**
