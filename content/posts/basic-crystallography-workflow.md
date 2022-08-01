---
author: "Horst Puschmann"
title: "The basic crystallographic workflow"
date: "2022-07-31"
description: "How a structure is typically obtained"
tags: ["crystallography", "small-molecule", "structure solution", "data reduction", "structure refinement"]
categories: ["QuantumBox"]
ShowToc: true
---

## The Basics

In crystallography, a crystal of a sample is subjected to X-ray or neutron radiation. This radiation interacts with the regular arrangement of the atoms in the crystalline material, and, in doing so, some of the incoming radiation is scattered (diffracted) in a specific way. By recording the diffraction pattern carefully, the exact arrangement of the atoms in the material that the crystal is made of can be deduced in a complicated series of operations.



{{< mermaid >}}
graph LR
    classDef s1 fill:orange,stroke:#333,stroke-width:0px;
    classDef s2 fill:lightgray,stroke:#333,stroke-width:0px;

0(Diffraction Measurement)
0 --> A1(Solution & Refinement) --> A2(Properties)
    class 0,A2 s2;
    class A1 s1;
{{< /mermaid >}}




### Diffraction Measurement

The diffraction measurement (sometimes called *data collection*) happens on sophisticated hardware, the [diffractometer](/glossary/#diffractometer). The crystal is mounted on this machine, X-rays are switched on and the diffraction that occurs because of the regular arrangement of the atoms in the crystal consists of diffracted (or scattered) X-rays. This pattern is collected in a series of images (also called *frames*).

These frames contain *spots* -- whenever a diffracted X-ray hit the detector, there will be a signal.

 - The position of the diffracted spots depends *only* on the dimensions of the [unit cell](/glossary/#unit-cell).
 - The stronger the signal, the more intense that particular diffracted beam was. Fom the intensity of these spots, we can determine the actual contents of the unit cell.

Condensing all the information contained in these hundreds (or thousands!) of frames down to a useful format is called the *data integration* or *data processing* step of the structure analysis.

---

### Solution & Refinement

Once we've got a list of all these diffraction spots, together with their measured intensities and an estimate of the error associated with each measurements, we can progress to the next step.

#### Structure Solution

In this ste


<br>

---
