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


## Module 3: Set Optimisation
The third and final module required in the final product requires the design of another interface around the third program in the Primacy pipeline. This part of the pipeline focuses on providing further optimisation to the output from the previous step of the pipeline, and providing a set of usable primers usable for genetic similarity analysis. This step has the following inputs:


1. Max number of iterations for optimization.
2. Optimum amplicon size range. This will help pick primer pairs that will produce an amplicon in this size range.
3. Max distance of target from a primer. If the amplicons are going to be sequenced, the target should be with the sequencing platforms read length. 
    * Distance from forward primer
    * Distance from reverse primer
    * Distance from at least one primer
    * Distance from both primers
4. Background Primers
5. Relative importance of features
    * Similar melting temperatures: minimizes the variation in melting temperatures for primers in the set
    * Primer scores: minimizes the individual primer scores for primers in the set to favor high ranking primers
    * Cross dimerization: minimizes the number of cross interactions between all primers
    * Amplicon size: minimizes distance outside of range of optimal amplicon size
    * Target distance from primer: minimizes distance of primer from target
6. Include primers/exclude primers


The group has planned to make these inputs interactable by the user by using the plan outlined in this diagram:


**TODO: Diagram**
