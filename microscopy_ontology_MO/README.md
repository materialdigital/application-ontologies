# Microscopy Ontology (MO)
This repository contains the [Microscopy Ontology (MO)](https://github.com/materialdigital/application-ontologies/blob/main/microscopy_ontology_MO/pmd_mo.ttl) and related information. The MO has been developed as part of the Platform MaterialDigital [(PMD)](https://materialdigital.de/) project in collaboration with the National Institute of Standards and Technology ([NIST](https://www.nist.gov/)).

Designed as an application ontology, the MO imports and builds upon the PMD Core Ontology ([PMDco](https://github.com/materialdigital/core-ontology/tree/main)), a mid-level ontology for materials science and engineering ([more details here](https://doi.org/10.1016/j.matdes.2023.112603)), and extends the PMDco with approx. 200 terms retrieved from an NLP approach by analyzing 2 decades of [Microscopy and Microanalysis Conference](https://microscopy.org/past-m-m-meetings) proceedings.

For further details, see:

### Scientific Publication

When using and referring to the Microscopy Ontology (MO), please cite the following publication, which provides comprehensive details and the foundational rationale behind the development of this ontology:

*Bayerlein, B., Schilling, M., Curran, M. et al. Natural Language Processing-Driven Microscopy Ontology Development. Integr Mater Manuf Innov (2024). https://doi.org/10.1007/s40192-024-00378-y*

Bibtex:
```
@article{Bayerlein2024,
  author = {Bernd Bayerlein and Markus Schilling and Maurice Curran and Carelyn E. Campbell and Alden A. Dima and Henk Birkholz and June W. Lau},
  title = {Natural Language Processing-Driven Microscopy Ontology Development},
  journal = {Integrating Materials and Manufacturing Innovation},
  year = {2024},
  doi = {10.1007/s40192-024-00378-y},
  url = {https://doi.org/10.1007/s40192-024-00378-y},
  issn = {2193-9772}
}
```
available open access at: [Integrating Materials and Manufacturing Innovation](https://doi.org/10.1007/s40192-024-00378-y).

**Note: This repository contains the PROV-O compatible MO version (referring to [PMDco 2.0.8](https://github.com/materialdigital/core-ontology/releases/tag/v2.0.8)). For the newest BFO-compatible MO version, please refer to the [microscopy ontology repository](https://github.com/materialdigital/microscopy-ontology).**

## Scope 
The Microscopy Ontology (MO) extends the ontological framework of the PMDco v2.0.7 as an [application ontology](https://github.com/materialdigital/application-ontologies). The MO facilitates semantic integration and the interoperable connection of diverse data sources from the fields of microscopy and microanalysis. Consequently, the MO paves the way for new, adaptable data applications and analyses across various experiments and studies ([Click here for more info](10.1038/s41597-024-03169-4)).

MO serves as a crucial foundation for annotating (meta)data in microscopy and microanalysis. With the MO, such data can be seamlessly transformed into RDF formats for advanced data management. This simplifies the understanding and communication between humans and machines and also boosts the data's interpretability, findability, and reusability, significantly contributing to research transparency and reproducibility.

By formalizing specialized knowledge about instruments, techniques, and related aspects, the MO facilitates the application of codified human knowledge in machine-driven processes. This enhances informed, automated decision-making, leading to better data interpretation, hypothesis generation, and experimental design. Moreover, these knowledge representations promote a sustainable, data-centric approach and hold the potential to further the development of large language models.

MO incorporates the most commonly used and, therefore, pivotal terms and abbreviations within the professional community. As a standardized structure, the MO allows for easy customization to suit individual needs by adding extra (meta)data classes specific to particular techniques and instruments, already identified in various output formats like dm3, tiff, and more.

Developed as a prototype for swift application ontology creation, MO employs a reproducible and transferable approach based on a specialized community text corpus using natural language processing (NLP) techniques and tools. This corpus includes contributions from two decades of the Microscopy and Microanalysis Conference, with the derived terms being categorized according to PMDco.

In addition to the increased speed of the methodology, the attractiveness of this method for other areas is that it can potentially circumvent special interests and individual biases. The methodology can therefore be reapplied at regular intervals to reflect the fact that our technology, and therefore language, is constantly evolving. As a result, the ontology and its subsequent versions evolve into dynamic representations of the field's accumulated knowledge.

## Documentation
An HTML documentation of MO that was auto-generated using [Widoco tool](https://github.com/dgarijo/Widoco) implemented as an GitHub action can be found at the [gh-pages of MO](https://materialdigital.github.io/application-ontologies/mo/index-en.html) and using the MO namespace [https://w3id.org/pmd/mo](https://w3id.org/pmd/mo).

## Contribute
An open [MO HackMD document](https://hackmd.io/21tFuZTITq2draxRPbepzg) used for collaborative work on shared vocabulary / thesaurus used for [pmd_mo.ttl](https://github.com/materialdigital/application-ontologies/blob/main/microscopy_ontology_MO/pmd_mo.ttl) is available. Please feel free to contribute but highlight changes in the thesaurus.

## Namespaces
In this section, the namespaces used in the Microscopy Ontology (MO) are listed. These can also be found in the [pmd_mo.ttl file](https://github.com/materialdigital/application-ontologies/blob/main/microscopy_ontology_MO/pmd_mo.ttl).
Since MO imports the PMDco, the PMDco namespace (https://w3id.org/pmd/co/) is used for higher-level ontological concepts.
The base of the MO (IRI of the ontology and of single concepts) is https://w3id.org/pmd/mo/. 

| Prefix | Namespace / URI                             |
|:-------|---------------------------------------------|
| :      | https://w3id.org/pmd/mo/                    |
| owl    | http://www.w3.org/2002/07/owl#              |
| rdf    | http://www.w3.org/1999/02/22-rdf-syntax-ns# |
| xml    | http://www.w3.org/XML/1998/namespace        |
| xsd    | http://www.w3.org/2001/XMLSchema#           |
| rdfs   | http://www.w3.org/2000/01/rdf-schema#       |
| base   | https://w3id.org/pmd/mo/                    |
