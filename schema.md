---
component-id: rulebook-schema
name: Ecosystem Component Annotation Schema
description: the Ecosystem Component Annotation Schema
type: Schema
work-package:
- WP1
licence: 
- Cc010Universal
related-components:
- reuses:
  - "Ecosystem Annotation Schema https://github.com/reeco-framework/reeco-annotation-schema/blob/main/schema/README.md"
- extends:
  - rulebook
--- 
# Ecosystem Component Annotation Schema

A complete list of component and container types and related annotation terms can be found in the [reference documentation](https://github.com/reeco-framework/reeco-annotation-schema/blob/main/schema/README.md).

## Use the schema 

### Components
Just copy the YAML code below and use it as the header of your component description MD file by changing terms values and removing terms that are not needed.
```
---
component-id: fabulous-component-source-code
type: Software
name: The Fabulous Source Code
description: Source code of The Fabulous
image: https://www.example.org/image.png
logo: https://www.example.org/logo.png
work-package: 
- WP1
- WP2
- WP3
- WP4
- WP5
- WP6
- WP7
- WP8
pilot:
- TUNES
- BELLS
- INTERLINK
- MUSICBO
- TONALITIES
- MEETUPS
- CHILD
- ORGANS
- ACCESS
- FACETS
project: polifonia-project
resource: https://github.com/fabulous-inc/repo1/releases
demo: https://www.example.org/fabulous/demo
release-date: YYYY/MM/DD
release-number: v1.0-alpha
release-link: https://github.com/polifonia-project/repo1/releases/tag/v1.0
doi: 10.5281/zenodo.000000
changelog: https://github.com/polifonia-project/repo1/releases/tag/v1.0
licence:
- CC-BY_v4
- CC-BY-SA_v4
- CC-BY-NC-ND_v4
- Apache-2.0
copyright: "Copyright (c) 2023 The Polifonia Project Contributors"
contributors:
- A developer <http://www.example.org>
- Another contributor <name.surname@example.com>
related-components:
- informed-by:
  - fabulous-requirements
- use-case:
  - fabulous-uc
- story:
  - fabulous-story
- persona:
  - fabulous-persona
- documentation: 
  - fabulous-component-docs
  - fabulous-component-tutorials
- evaluated-in:
  - fabulous-evaluation
- extends:
  - "A Java project Jena https://www.example.org"
- reuses:
  - "Apache Camel https://camel.apache.org/"
  - another-dataset
- serves:
  - another-dataset
- generated-by:
  - The AI code generator http://www.my-software-factory.com
- derived-from:
  - this-other-component
credits: "This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement N. 101004746"
--- 
```


### Containers
Just customise the YAML code below and use it as the header of your component description MD file by changing terms values and removing terms that are not needed. 

```
container-id: fabulous
name: The Fabulous Project
description: The Fabulous Project is a very important part of the Polifonia ecosystem.
type: Project
work-package: 
- WP1
- WP2
- WP3
- WP4
- WP5
- WP6
- WP7
- WP8
pilot:
- ThePilot
project: polifonia-project
bibliography:
- main-publication: "Brown, L. (2019). The Role of Parenting Styles in Child Development. Child Development Perspectives, 13(3), 145-153."
- publication: 
  - "Smith, J. (2020). The Impact of Social Media on Mental Health. Journal of Psychology and Behavioral Sciences, 15(2), 45-62."
funder:
  - name: Horizon 2020 Framework Programme
    url: https://cordis.europa.eu/programme/id/H2020-EC
    grant-agreement: "https://cordis.europa.eu/project/id/101004746"
credits: "This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement N. 101004746."
has-part:
  - fabulous-component-source-code
  - fabulous-docs
  - fabulous-tutorials
  - fabulous-evaluation
  - fabulous-requirements
  - fabulous-dataset

```
