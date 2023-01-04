---
component-id: ontology-rulebook
name: Ontology and knowledge graph development and documentation guidelines
description: The guidelines for the development and documentation of an ontology and a knowledge graph
type: Schema
release-date: TBD
release-number: v1.0
release-link: 
work-package:
- WP2
pilot:
- BELLS
- ORGANS
- MEETUPS
- MUSICBO
- CHILD
- TONALITIES
keywords:
  - Ontology/KG development
  - Ontology/KG documentation
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

# Ontology and knowledge graph development and documentation guidelines


## Ontology development and documentation guidelines

### Ontology development guidelines
 - The namespace of the ontology (published within the Polifonia Ontology network) must follow this rule:
    - Rule: https://w3id.org/polifonia/ontology/[name-of-the-ontology
    - Example: https://w3id.org/polifonia/ontology/musical-composition

- The ontology should be annotated with labels (rdfs:label) and comments (rdfs:comment).
- The ontology should contain alignments to possible ODPs reused through [OPLaX ontology](https://w3id.org/OPLaX).
  - See an example of an ontology annotated with the reused patterns here: https://github.com/ICCD-MiBACT/ArCo/blob/master/ArCo-release/ontologie/catalogue/1.2/catalogue.owl

- The ontology should contain alignments to possible ontologies produced by partners of Polifonia and reused within the project.

### Ontology documentation guidelines

- Each ontology (published within the Polifonia Ontology network) should be stored as an RDF/OWL file in a GitHub repository. 
  - The name of the repository should follow this rule: 
    - Rule: [name-of-ontology]-ontology
    - Example: https://github.com/polifonia-project/musical-performance-ontology
- The documentation of the ontology in the README.md file:
  - The README.md file must contain a brief description of the scope of the ontology.
  - The README.md file should contain useful statistics about the ontology in order to give an overview (number of classes, number of properties, ...)
  - The README.md file should contain examples of relevant Competency Questions with respective SPARQL queries
  - The README.md file should contain a graphical representation of classes and predicates.
  - The README.md file should contain the licence for the reuse (hence responsible people).

- The repository should include a separate folder containing ontology tests following eXtreme Design methodology (it is recommended to use the XDTesting tool).
- For each ontology produced by partners of Polifonia and reused within the project, but published outside the Polifonia Ontology Network, it should exist a repository linking to the ontology.
- Information about the ontology must be added/updated in the [Network Ontology GitHub repository](https://github.com/polifonia-project/ontology-network}{network-ontology).

## Knowledge graph development and documentation guidelines

### Knowledge graph development guidelines

- The namespace of the knowledge graph (published within Polifonia) needs to follow the rule:
  - Rule: https://w3id.org/polifonia/resource/[class-local-name]/[SHA-1 hash function of the unique attribute(s) of the individual]
  - Example: https://w3id.org/polifonia/resource/Score/ec68f1e4727ecdd5272d247f3e3176743e38b469 for an entity of type Score, with the hash generated from the concatenation of the title and the composer of the composition of the score
- The knowledge graph should contains links (owl:sameAs) to the Wikidata knowledge graph. 
- The knowledge graph needs to be deployed on the web through a SPARQL endpoint containing all relevant prefixes.

### Knowledge graph documentation guidelines

- The knowledge graph must be documented in a GitHub repository, that follows the rules already defined in the [Polifonia rulebook](https://github.com/polifonia-project/rulebook/) valid for all GitHub repositories.
- The documentation of the ontology in the README.md file:
  - The README.md file must contain a brief description of the scope of the knowledge graph. 
  - The README.md file should contain the link to the SPARQL endpoint
  - The README.md file should contain useful statistics about the KG (number of triples, most populated classes, ...)
  - The README.md file should mention the data sources of the KG
  - The README.md file should contain examples of relevant Competency Questions with respective SPARQL queries
  - The README.md file should contain the licence for data reuse (hence responsible people).
- A copy of data (Linked Open Data) should be linked in a dedicated folder in the repository. If the data volume exceeds 500MB, split data into different files. If data are difficult to split, use [ntriples](https://heardlibrary.github.io/digital-scholarship/lod/serialization) / [quads](https://www.w3.org/TR/n-quads/) serialisation. Otherwise, any.
- A story created with Melody, containing relevant queries that can be run on the knowledge graph, should be present in the documentation. At least one query should showcase the entity linking with Wikidata.


