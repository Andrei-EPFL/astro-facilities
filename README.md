# RDF Ontologies for Astronomical Data and Workflows

This repository contains two RDF ontologies that include astronomical concepts and workflows. Slightly different versions of these ontologies are used in a [MMODA](https://www.astro.unige.ch/mmoda/) workflow, [analyse-short-astro-text](https://gitlab.renkulab.io/astronomy/mmoda/analyse-short-astro-text). Both should be part of the main [ODA ontology](https://odahub.io/ontology/)

## Ontologies

1. [**Astro-Facilities Ontology:**](astro-facilities.ttl)  
   This ontology focuses on concepts such as: telescopes, observatories, surveys, and space telescopes.

2. [**MMODA-Workflows Ontology:**](mmoda-workflows.ttl)  
   This ontology captures the [MMODA](https://www.astro.unige.ch/mmoda/) workflows (publicaly available on the 25th of November 2024) and their relationship to the instruments captured in the previous ontology.

## Standards and Resources

The ontologies build upon widely-used vocabularies and ontologies in the semantic web and astronomical domains, ensuring alignment with existing standards:

- [Dublin Core Terms](http://purl.org/dc/terms/)
- [OWL Web Ontology Language](http://www.w3.org/2002/07/owl)
- [RDF Schema (RDFS)](http://www.w3.org/2000/01/rdf-schema)
- [SKOS (Simple Knowledge Organization System)](http://www.w3.org/2004/02/skos/core)
- [IVOA Messenger Ontology](http://www.ivoa.net/rdf/messenger)
- [IVOA UAT Ontology](http://www.ivoa.net/rdf/uat)
- [ODA Ontology](https://odahub.io/ontology)

## New Classes and Properties

The ontologies introduce four new classes and one object property to enhance the existing semantic structure:

### New Classes:
1. **`misctelescope`**  
   A class for entities that are not obviously described by the other categories (8 entities).
   
2. **`telescope-class`**  
   A class defining different categories of telescopes based on their characteristics and functionalities, e.g. Corrected Dall Kikham (CDK) or Schmidt telescopes (10 entities).

3. **`institution`**  
   Represents organizations or institutions that manage or operate astronomical facilities (11 entities).

4. **`observatory`**  
  A concept related to the [**`observatories`**](https://www.ivoa.net/rdf/uat/2024-06-25/uat.html#observatories) concept. In practice, for simplicity, all entities that include in their name the word "Observatory" are classified as **`observatory`** (129 entities).

### New Object Property:
- **`canDetect`**  
  Relates an entity (e.g., a telescope or survey) to the type of messengers it can detect, as defined in the [IVOA Messenger Ontology](http://www.ivoa.net/rdf/messenger) and [IVOA UAT Ontology](http://www.ivoa.net/rdf/uat) for the gravitational waves.

## Other classes:
1. **`http://www.ivoa.net/rdf/uat#telescopes`** (292 entities)
2. **`http://www.ivoa.net/rdf/uat#surveys`** (85 entities)
3. **`http://www.ivoa.net/rdf/uat#space-telescopes`** (123 entities)
4. **`http://www.ivoa.net/rdf/uat#refracting-telescopes`** (17 entities)
5. **`http://www.ivoa.net/rdf/uat#radio-telescopes`** (60 entities)
6. **`http://www.ivoa.net/rdf/uat#radio-interferometry`** (1 entity)
7. **`http://www.ivoa.net/rdf/uat#neutrino-telescopes`** (3 entities)
8. **`http://www.ivoa.net/rdf/uat#astronomical-instrumentation`** (46 entities)

## Contributing

Contributions are welcome! If you have suggestions for improvements or extensions, please open an issue or submit a pull request.
