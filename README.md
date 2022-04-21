---
component-id: rulebook
name: Ecosystem Development Rulebook
description: Guidelines, recommendations, and norms on how to contribute to the Polifonia Ecosystem.
type: Documentation
release-date: 21/04/2022
release-number: v1.0
work-package: 
- WP1
licence: Public domain, https://unlicense.org
links:
- https://github.com/polifonia-project/rulebook
credits:
- https://github.com/enridaga
- https://github.com/raphaelfournier
---
# Rulebook
Guidelines, recommendations, and norms on how to contribute to the Polifonia Ecosystem.

## Guidelines
### When to create a repository? 
Create a GH repository whenever there is an activity which leads to the production of a *component* of the *Polifonia Ecosystem*.  

### Do I really need to create a repository for anything I do? 
No. But as soon as the work is discussed or presented in a meeting a repository should be already there, or follow straight after! 
A repository with annotated component descriptions (see later) is mandatory for components mentioned in official deliverables. 

### What if a repository already exists somewhere else? 
You don’t need to fork the repository in the Polifonia organisation. External components can be described (with annotations) in the repository [external-components](https://github.com/polifonia-project/external-components/). 

### Champion 
Each repository must have a champion. Champions need to be annotated in the [CHAMPIONS.md](CHAMPIONS.md) file.

### Discussion and decisions 
Discussions can happen anywhere at anytime. However, decisions that impact the development of the component **MUST** be logged within an Issue (a Github issue, example) and motivated. 

If the decfision is not being recorded in an Issue, **it never happened**. 

### Tracking changes (commits) 
Commit messages are mandatory and must reference at least one Issue. A good commit message is `Added folder XYZ with data from QWE, see also #432` where `#432` is the issue number in the same repository. You can also reference any URL in commit messages, please see GitHub documentation for examples. The more you link, the better. 

Useful readings on best practices:

 - https://gist.github.com/luismts/495d982e8c5b1a0ced4a57cf3d93cf60#file-gitcommitbestpractices-md
 - https://medium.com/@danielfeelfine/commit-verbs-101-why-i-like-to-use-this-and-why-you-should-also-like-it-d3ed2689ef70

This is a [bad commit message](https://github.com/polifonia-project/rulebook/commit/78fb11bbe0fee670fea70dc3f3cf4bf096ab3513)
This is a [good commit message](https://github.com/polifonia-project/rulebook/commit/60dc07702fd6aaf86b029da0c5f873f77f36313e)

### Tracking Progress Issue
Progress on the development of each component MUST be reported in the Issues section periodically.
Each repository **SHOULD** have a single **Tracking Progress Issue** for general progress update.
A simple reporting template can be a bullet list in three sections: Progress, Problems, and Perspectives (3P).

The 3P are:

 - Progress: what concrete work has been done since the last update.
 - Problems: anything that is slowing or blocking progress, or it is expected to do so.
 - Perspectives: what progress is expected going forward, including plans that have been made to face any of the problems (if any).

Please note that the Tracking progress issue is only for updates. Detailed, task-based issues should be used for referencing changes (commits) and can be linked in the Tracking Progress Issue. 

Examples:

- [Tracking progress issue (Rulebook)](https://github.com/polifonia-project/rulebook/issues/7)
- [Tracking progress issue (External Components)](https://github.com/polifonia-project/external-components/issues/1)

### Naming conventions 
Some naming conventions have been discussed, feel free to contribute to the discussion [here](https://github.com/polifonia-project/rulebook/issues/2)

For repositories 

 - Avoid including “Polifonia” in the name (e.g. `ecosystem` rather then `polifonia-ecosystem`) 
 - Avoid acronyms (`ontology-network` instead of `ON`) 

### Branches 
Use branches for managing different versions of the code / components. Avoid creating a branch for each sub-system (e.g. /datasets /ui etc... Instead, create different repositories. 

### Releases 
Use Semantic Versioning for release numbers, and follow the GitHub workflow for releasing.

Register your repository on Zenodo, by activating the related GitHub Action. See [this guide](https://guides.github.com/activities/citable-code/).

## Contributing to the Ecosystem
### What is a Polifonia Ecosystem *component*? 
Basically, anything that is not a research paper, dissemination product (e.g., video presentation of a tool), or deliverable. 

List of component types: 

Documentation:
 - Persona (strictly from https://github.com/polifonia-project/stories)
 - Story (strictly from https://github.com/polifonia-project/stories)
 - Tutorial
 - Documentation

Executables:
 - Application
 - Container
 - Experiment
 - CLI tool
 
Reusable software:
 - Library
 - User Interface
 - Service

Data:
 - Registry
 - Ontology
 - Dataset
 - Repository
 - Corpus
 - Knowledge Graph

### Polifonia Ecosystem Website
A repository contains the development work for at least 1 component in the **Polifonia Ecosystem**. One markdown text file should expose annotations (metadata) relative to a single component included in the repository. For example, a component-name.md file using the annotation schema of the Polifonia Ecosystem (the file can have any name). A repository can include multiple annotated files, hence expose multiple components. 
Those annotations will be used by the [Polifonia Ecosystem website](https://github.com/polifonia-project/ecosystem). 
This website will provide a user interface for navigating through the Polifonia Ecosystem (with aggregation pages, tags, etc). 
Please note that the Polifonia ecosystem website uses the content of Github repositories as is, hence the need for good quality annotations / documentation.  

### Developing Schema Components Annotations 
The annotations should be written at the top of the markdown file, between 2 “---” lines. The markup format is YAML (mostly a “key: value” format, see also example at the top of this file). The schema to follow is [this one](schema.md). Developers can use this service to test the YAML code:  https://jsonformatter.org/yaml-validator .

### Process towards ecosystem releases

- Champions curate releases with project-specific frequency and rationale
- - Releases must be linked to Zenodo and the related Polifonia Community
- TB calls for next Ecosystem Release
- Champions reply giving details about version number and expected deadline (if any)
- Champions ensure component metadata is accurate
- Ecosystem Website prepare release candidate
- TB tests and validates Ecosystem Website release candidate
- Ecosystem released

## How to contribute to the Rulebook
Please open an issue with proposals or questions about the rulebook!
