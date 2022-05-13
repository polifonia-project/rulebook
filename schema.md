---
component-id: rulebook-schema
name: Ecosystem Component Annotation Schema
description: the Ecosystem Component Annotation Schema
type: Schema
release-date: 21/04/2022
release-number: v1.0
release-link: 
work-package:
- WP1
pilot:
keywords:
  - Ecosystem
changelog:
licence:
release link:
image:
logo:
demo:
links: 
running-instance:
credits: 
related-components:
  - Rulebook
bibliography:   
--- 
# Ecosystem Component Annotation Schema

## Use the schema 

Just copy the YAML code below and use it as the header of your component description MD file.
```
---
component-id:
name:
description:
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
 - component-id-1
 - component-id-2
bibliography: 
  - oneref
  - another ref
  
--- 
```

See below for a description of the fields and expected values.

## Description of fields 

| Name | Description | Format/Example |
|------|-------------|----------------|
| component-id | Identifier of the component | lowercase |
| name | Full name of the component | Text (no size limit) |
| description | A brief description of the component | 100 word max. |
| type | Type of component | one of: Tutorial, Documentation, Application, Container, Experiment, CLI, Library, User, Interface, Service, Registry, Ontology, Dataset, Repository, Corpus, "Knowledge Graph" |
| release-date | Date of the release | 2021-09-28 (ISO 8601) |
| release-link | Link to the release | https://github.com/SPARQL-Anything/sparql.anything/releases/tag/v0.5.1 |
| release-number | Version number for the current release | v0.1 |
| work-package | Relevant WPs (list) | [ WP1, WP2 ] |
| pilot | Pilot identifiers | [ FACETS, TUNES ] |
| keywords | List of keywords (max 8) | <ul><li>keyword1</li><li>keyword2</li><li>...</li></ul> |
| changelog | Link to a document specifiying the changes between this and the previous version | URL |
| licence | A licence for the code | MIT, GPLv3. A link may be provided: [Unlicense](https://unlicense.org/) |
| release-link | A link towards a release archive/image | URL |
| image | A presentation image (JPEG, PNG, etc.) | URL |
| logo | A logo for the component (JPEG, PNG, etc.) | URL |
| demo | A demontration for the component (e.g., video tutorial) | A link for the demo |
| links | A list of relevant web links | List of URLs <ul><li>http://onelink.com </li><li>http://www.anotherone.com </li></ul> |
| running-instance | A link towards a running instance of the component | URL |
| credits | Names of people participating in the developement | E. Daga (OU), R. Fournier-S'niehotta (CNAM) |
| related-components | Relevant components | [ component-id1, component-id2, ... ] |
| bibliography | Relevant publications | List of references |

## Information that can be automatically derived

- Statistics such as number of commits 
- Contributors (number of them or list of them) 
- Creation date 
- Number of releases 
- Size 
- Programming language 
- Link to repository, issues, etc … 
- Citation 
