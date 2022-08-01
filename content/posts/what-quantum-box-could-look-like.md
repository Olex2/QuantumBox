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

Striaghforward doesn't mean easy: the measurements must be performed with the greatest care and there are limitations due to the technology available at the time. And diffractometers have steadily improved over the decades: the data quality achievable nowadays is truly outstanding.

Alongside the development of better diffractometers, computing power has also increased enormously during the 50 years (or so) during which routine structure analyses have been carried out.