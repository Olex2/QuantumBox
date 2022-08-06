---
author: "Horst Puschmann"
title: "Alternative Workflows"
date: "2022-08-06"
description: "The new home of small-molecule crystallography"
tags: ["crystallography", "small-molecule", "crystal structures", "workflow"]
categories: ["QuantumBox"]
ShowToc: true
---

In the typical crystallographic workflow, there are often points at which many alternative ways of achieving a particular goal are possible. Some of these ways may be 'better' than others, some may be faster than others, and not all will lead to the same end point.

## Example 1: Structure Solution

Here is an example where there are many different programs that can be used to perform the steop of the initial [structure solution](/glossary/#structure-solution).

{{< mermaid >}}
graph TB
    classDef s1 fill:orange,stroke:#333,stroke-width:0px;
    classDef s2 fill:lightgray,stroke:#333,stroke-width:0px;

0(Output from data reduction)
O(Structure solution)
0 -.-> A1(ShelXT) -.-> O
0 -.-> A2(ShelXD) -.-> O
0 -.-> A3(ShelXS) -.-> O
0 -.-> A4(Superflip) -.-> O
0 --> A5(olex2.solve) --> O
0 -.-> A6(SIR) -.-> O
    class 0,O,A1,A2,A3,A4,A6 s2;
    class A5 s1;
{{< /mermaid >}}

It is not important *how* we arrive at the structure solution, as long as we find the correct solution. Depending on the nature of the problem, some of these programs may be be faster, or may have a larger chance of success, than others.

Apart from olex2.solve, which is an integral part of Olex2, all of these programs are stand-alone programs, all with their own input and ouput formats. It is far from easy to 'just try them all', unless the process is somehow managed.

In this example, it ultimately irrelevant *how* the solution was arrived at, but it is still important to somehow catpure the actual path taken that lead to the initial solution from which the rest of the structure determination proceeded.


## Example 2: Structure Refinement

In this example, we are now looking at the next step in the process of structure determination: the refinement step. Again, there are different programs available that will do the job -- and we are facing the same problems as before: they each come with their own input and output formats which are largely incompatible.

{{< mermaid >}}
graph TB
    classDef s1 fill:orange,stroke:#333,stroke-width:0px;
    classDef s2 fill:lightgray,stroke:#333,stroke-width:0px;

0(Input Model)
O(Refined Output Model)
0 -.-> A1(ShelXL) -.-> O
0 -.-> A2(olex2.refine) -.-> O
0 -.-> A3(CRYSTALS) -.-> O
0 -.-> A4(JANA) -.-> O
0 --> A5(REALS) --> O
    class 0,A1,A5,A3,A4,A6 s2;
    class A2 s1;
{{< /mermaid >}}

But there is now an important difference: the resulting models will all be slightly different from each other, and these differences *matter*. While all the above programs will perform, broadly, some 'Least Squares Minimisation', they all do this in subtly differnet ways -- and even within each program there are many many different settings that can be applied.







