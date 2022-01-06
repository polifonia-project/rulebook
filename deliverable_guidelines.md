# Polifonia Software Deliverable Guidelines

<aside>
ℹ️ Please, consider the following guidelines if your deliverable is of type **OTHER/SOFTWARE**.

</aside>

# Table of contents

 * [Report](#report)
    * [Summary](#summary)
    * [Exploitability](#exploitability)
    * [Future work](#future-work) 
 * [Github](#github)
    * [Checklist](#checklist)
    * [Github documentation](#github-documentation)
    * [Testing](#testing) 

# Report

**For each software** described in the deliverable, include the following three sections: **Summary**, **Exploitability, Future work**. 

### Summary

A table including the following fields, partly based on the [schema.md](http://schema.md) in the rulebook ([link](https://github.com/polifonia-project/rulebook/blob/main/schema.md)).

```yaml
---
id: either a Zenodo DOI or any other persistent handler
type: Software | Data
title: attibuted title of the software
credits: authors and contributors
description: a short abstract (goal, motivation, problem, future and current evaluation methods) max 200 words
source code: the URL of the source code
documentation: link to documentation of the software (e.g. README.md)
release: link to either release or pre-release
licence: if restrictive license, you are required to explain why
running instance: e.g. a demo, a web app based on the software, a jupyter notebook showing how to run the code and few examples of usage
bibliography: peer-reviewed works or reports in which the software is presented. 
related deliverables: link to Polifonia deliverables (e.g. reports) in which methods/software are detailed or relevant (see comment below)
---
```

*NOTE: In **related deliverables,** include as many references as possible to documents (deliverables or online documentation) that:*

- *detail methods used by the software and/or to create the data*
- *reuse the software/dataset (e.g. deliverables by other partners that reuse your work - or are going to)*

*When including the link to documents, please briefly explain what aspects these documents address, e.g. `DX.X (full description of methods, context of usage); DY.Y (software reuse in task Z.Z)`*

### Exploitability

- Make clear the interconnection between the software and the overall project objectives
- Introduce the context in which the software / dataset is used (the task and the partners)
- Explain who is going to benefit from it (partners in Polifonia, potential re-users, stakeholders already identified).

*NOTE: if the software / dataset is already detailed in another deliverable, this report can be just a short reminder, in case different reviewers are assigned to deliverables. In any case, provide all the necessary context information needed to understand your work without expecting the reviewer to dive into your code base.*

### Future work

- detail how you intend to **continue developing** the software component or enriching the dataset
- explain **evaluation** methods, even if not implemented yet

---

# Github

Please, make sure that your repository complies with [the rulebook](https://github.com/polifonia-project/rulebook), follow instructions in the **Checklist** and add suggestions for the **Documentation** on the repository.

## Checklist

- include the following header to make it findable by the [Polifonia ecosystem](https://github.com/polifonia-project/ecosystem).

```yaml
---
id: 
name:
brief-description:
type:
release-date:
release-number:
work-package:
pilot:
keywords:
  - kw1
  - kw2
changelog:
licence:
release link:
image:
logo:
demo:
links:
  - link
running-instance:
credits:
related-components:
  - dataset
    - component-id-1
    - component-id-2
  - cli
    - cli-component-id1
    - cli-component-id2
  - stories

bibliography:
  - oneref
  - another ref

---
```

- by the due date of the deliverable you must deposit the Github repository on **Zenodo** (see guidelines to start [Zenodo-github]() sync)
- make a release of the code (so that the Zenodo sync can start)
- include the **DOI** of Zenodo in evidence in the `README.md` file of the repository and in the **report**
- include the **license** (e.g. a comment in the code or in the `LICENSE.md` file, see [guidelines](https://www.freecodecamp.org/news/how-open-source-licenses-work-and-how-to-add-them-to-your-projects-34310c3cf94/))

## Github documentation

Please, refer to [Awesome-READMEs](https://github.com/matiassingers/awesome-readme) for a list of exemplar curated README files. 
Here a [good example of README file for software (librosa python library)](https://github.com/librosa/librosa) and a [minimal template of README file for datasets](https://gist.github.com/shashvatshah9/5d587605cd087182ccffb46b6cf9e449)

The documentation should include the following sections.

### Introduction

- abstract and highlights of the software
- reference to Polifonia deliverable of type OTHER/SOFTWARE (name and URL if available)
- citation of the software repository
- license
- Zenodo DOI

### Information on installation and setup

- either package **requirements** (e.g. `requirements.txt`)
- or add instructions to recreate the software environment (e.g. conda environment, docker, installer)
- [if applicable] list data sources to be downloaded (with links)

### Running and examples

- Instructions on how to **run the code**
- add either a **Jupyter notebook** or **code samples** with examples on how to run the code, features, and output - so that the reviewer sees exactly what you want her/him to see and avoid them to dive into the code

## Testing

<aside>
🚧 Work in progress: testing guidelines are currently optional — but recommended!

</aside>

 It is good practice to start planning for testing from the very first moment the software component is engineered — before any actual coding takes place. Designing **test cases** for each function-method that is implemented, together with a simple framework allowing for their automatic execution is desirable. Nevertheless, the way the testing strategy is implement pretty much depends on the type of software that is developed. Therefore, this last guideline is more of an invitation to deliver a testing methodology, as part of the codebase, rather than enforcing a specific strategy. Regardless of the software-specific methodology, please make sure to provide all the relevant instructions to configure and run the testing scripts.
