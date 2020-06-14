#AMITT

## The AMITT Misinformation Framework

AMITT (Adversarial Misinformation and Influence Tactics and Techniques) is a framework designed to give responders better ways to rapidly describe, understand, communicate, and counter misinformation-based incidents.

AMITT is part of our work on adapting information security (infosec) practices to help track and counter misinformation. AMITT is designed to fit existing infosec practices and tools as closely as possible, giving responders the ability to transfer other information security principles to the misinformation sphere, and to plan defenses and countermoves.

The latest version of AMITT is held in the [AMITT Framework Github repository](https://github.com/cogsec-collaborative/amitt_framework)

## Describing a Misinformation Incident with AMITT

The language and style of the AMITT framework is adopted from the MITRE ATT&CK framework. The framework is read left-to-right in time, with the entities to the left typically (but not necessarily) happening earlier in an incident. The phases are separated into left-of-boom (purple) and right-of-boom (red), to represent activities before (left) and after (right) an incident is visible to the general public.

Every AMITT component has a unique id (e.g. T0018 Paid targeted ads). To use AMITT, list and share the components you see in your incident, e.g.:

* Phases (top row: purple and red boxes): higher-level groupings of tactics, created so we could check we didn't miss anything. The tactics below each phase belong to that phase.
* Tactics (second row: blue boxes): stages that someone running a misinformation incident are likely to use
* Techniques (all other rows: grey boxes): activities that an incident creator might use at each stage. The techniques below each tactic belong to that tactic.
* Tasks (not shown): things that need to be done at each stage. Tasks are things you do, techniques are how you do them.

Compiling and reporting incidents is an important aspect of both responding and developing the tools needed to do so. To be effective, those reports should include as much information as possible about the stages and techniques at play in those incidents. We’ve created an html tool to help you with this ([matrix-to-message](https://github.com/cogsec-collaborative/amitt_framework/blob/master/matrix_to_message.html)) - download it, and click on the boxes that you need in your report. You can then cut-n-paste the list of techniques that it generates at the bottom of the page.


## AMITT Extensions

AMITT is a living standard - the current model was built from an analysis of 22 incidents; the techniques listed are a subset of the ones used in misinformation incidents. The model will evolve -

* Refinement is an ongoing process,
* Learnings from AMITT’s use is an ongoing community feedback process,
* Naming conventions and descriptive changes to TTPs will/could evolve as AMITT adoption by responders and researchers expands

The current tool is the start of a larger toolset to implement the AMITT standard.
* We generated STIX templates for AMITT objects (repository [AMITT CTI](https://github.com/cogsec-collaborative/amitt_cti));
* so AMITT messages can be passed between ISAOs and similar bodies using infosec transport standards like TAXII; and
* so we can join these to STIX objects for misinformation artifacts from data scientists and other researchers.
