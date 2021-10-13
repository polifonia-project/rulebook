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

## Important notice 

```
Just copy the header of this file into yours!
```

See below for a description of the fields and expected values.

## Description of fields 

| Name | Description | Format/Example |
|------|-------------|----------------|
| id | Identifier of the component | lowercase |
| name | Full name of the component | Text (no size limit) |
| description | A brief description of the component | 100 word max. |
| type | Type of component | Pilot spec, Dataset, Ontology… |
| release-date | Date of the release | 2021-09-28 (ISO 8601) |
| release-number | Version number for the current release | v1.5 |
| work-package | Relevant WPs | WP1, WP2 |
| pilot | Pilot identifier | FACETS, TUNES |
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
| related-components | Relevant components, organized in lists by Types | <ul><li>Dataset</li><ul><li>Component-id1</li><li>Component-id2</li></ul><li>Stories</li><ul><li>Story1</li><li>Story2</li></ul></ul> |
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
