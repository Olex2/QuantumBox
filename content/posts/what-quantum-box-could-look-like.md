---
author: "Horst Puschmann"
title: "What could QuantumBox look like?"
date: "2022-07-31"
description: "The new home of small-molecule crystallography"
tags: ["crystallography", "small-molecule", "crystal structures", "method development"]
categories: ["QuantumBox"]
ShowToc: true
---

QuantumBox, as a project, has not started yet. We are currently in the design phase, and that is an exciting place to be.

---

## Structure Determination

X-rays (and some other radiation) will interact with a crystalline material in such a specific way, that it is possible to figure out what was in the crystal. We can determine where all the atoms are relatively to each other.

{{< mermaid >}}
graph LR
    classDef s1 fill:orange,stroke:#333,stroke-width:0px;
    classDef s2 fill:lightgray,stroke:#333,stroke-width:0px;

0(Diffraction Measurement)
0 --> A1(Solution & Refinement) --> A2(Properties)
    class 0,A2 s2;
    class A1 s1;
{{< /mermaid >}}

{{< som id="c3jVIrVZwNQ" >}}

Through a *pysical measurement*, we can obtain the *crystal structure* of a crystalline material. Once we have the structure, we can deduce many properties of the material, and that is often at the heart of why we perform a structure analysis in the first place.

> You can find more detail here: [crystallograpic workflow](/posts/basic-crystallography-workflow).


So, the process is straigthforward: we perform a physical measurement with the aim to deduce some chemical and physical properties of the material under investigation.

And not much has changed in terms of how structures are generally determined since structural analysis went 'mainstream' in the late 1970's.


## Better diffractometers, faster computers

Striaghforward doesn't mean easy: the measurements must be performed with the greatest care and there are limitations due to the technology available at the time. And diffractometers have steadily improved over the decades: the data quality achievable nowadays is truly outstanding.

Alongside the development of better diffractometers, computing power has also increased enormously during the 50 years (or so) during which routine structure analyses have been carried out.

![Moores Law](https://ourworldindata.org/uploads/2020/11/Transistor-Count-over-time.png)

### We can do better!

Despite these huge increases in the quality of the diffraction data as well as the available computing power, the very same techniques that have been used for over half a century are still used in all but very few specialist applications.

This all means that we are not making the most of our extremely good modern measurements -- the quality of crystal structures has not really improved over the years.

### ... but not for the want of trying!

Method development has continued throughout the history of crystallography, and those at the cutting edge could not wait for better experimental set-ups and faster computers to become available and affordable. [Synchrotron](/glossary/#synchrotron) facilities were built around the globe at astronomical expnese to this effect. The results that were obtained along every step were also stunning and have really helped our understanding of the nature chemical bonding along in a very big way.

### So, why are we stuck at the state-of-the-art of 50 years ago?

There are a number of reasons why much of 'routine' crystallography is largely still based on very old technology.

 - Better diffractomters are *always* available, but come at a cost.
 - Many practicing structural analysts do not wish to go much beyond a ['connectivity analysis'](/glossary/#connectivity-analysis) -- anything more would require extra effort
 - Software development is done by a few dedicated teams, and is mostly aimed at experienced users. It is probably fair to say that some crystallographic software can *only* be used by its author...
 - Interoperativity between software is often very difficult to achieve and requires many manual steps, which can be frustrating and error-prone.
 
All of the above lead to a certain amount of inertia. In an environment where results are required ever more quickly, there is often not enough time to get into something new: why deviate from a work-flow that has been working for so long?

