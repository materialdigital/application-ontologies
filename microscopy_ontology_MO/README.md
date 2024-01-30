# Microscopy Ontology (MO)

This repository comprises information on and files related to the microscopy ontology (MO) that was developed within the frame of the project 
Platform MaterialDigital [(PMD)](https://materialdigital.de/) in collaboration with [NIST](https://www.nist.gov/). 
It is designed as an application ontology by importing and thus making use of the mid-level PMD Core Ontology ([PMDco](https://github.com/materialdigital/core-ontology/tree/main)). Hence, it can be found within this [MO application ontology repository](https://github.com/materialdigital/application-ontologies/tree/main/microscopy_ontology_MO) as a part of the [PMD application ontology (PMDao)](https://github.com/materialdigital/application-ontologies/tree/main) repository.

## Scope 

The Microscopy Ontology (MO) is a comprehensive framework for representing knowledge that encompasses concepts from the domains of microscopy and microanalysis. The MO is semantically based on the mid-level PMD Core Ontology ([PMDco](https://github.com/materialdigital/core-ontology/tree/main)) to allow a connection to other MSE application ontologies and domain neutral concepts found in established top-level ontologies. The primary goal of MO is to provide a standardized vocabulary and framework for describing and organizing concepts, entities, and relationships within the field of microscopy and microanalysis. This standardization facilitates communication and interoperability between different systems, databases, and research groups. In order to obtain a vocabulary that is relevant in the field and therefore worth standardizing, an NLP approach was applied, with the help of which commonly used terms were determined. MO was then developed based on the respective list of terms. Microscopy and microanalysis generate vast amounts of data from various techniques and instruments. MO may help to integrate and link heterogeneous data sources, enabling the combination and analysis of data from different experiments and studies more effectively. Furthermore, MO serves as a basis for annotating microscopy and microanalysis data with standardized metadata. This improved metadata description enhances the interpretability, searchability, and reusability of data, promoting transparency and reproducibility in research. Moreover, by formalizing knowledge about instruments, techniques, materials, and phenomena, MO may provide the basis to enable machine reasoning to support data interpretation, hypothesis generation, and experimental design.
Overall, MO is intended to advance research, promoting collaboration, and facilitating knowledge exchange in this interdisciplinary domain.

## Documentation

An HTML documentation of MO that was auto-generated using [Widoco tool](https://github.com/dgarijo/Widoco) implemented as an GitHub action 
can be found at the [gh-pages of MO](https://materialdigital.github.io/application-ontologies/mo/index-en.html) and using the MO namespace [https://w3id.org/pmd/mo](https://w3id.org/pmd/mo).

## Contribute

An open [MO HackMD document](https://hackmd.io/21tFuZTITq2draxRPbepzg) used for collaborative work on shared vocabulary / thesaurus used for [pmd_mo.ttl](https://github.com/materialdigital/application-ontologies/blob/main/microscopy_ontology_MO/pmd_mo.ttl) is available. Please feel free to contribute but highlight changes in the thesaurus.

## Publication | Citation
When using and referring to the microscopy ontology (MO), please cite the following publication, which provides comprehensive details and the foundational rationale behind the development of this ontology:


Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed dapibus justo eget quam volutpat, ac fringilla nisl posuere. 

<!-- **Note:** This paragraph is under construction and will be updated soon with additional information. -->

Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.


## Namespaces
In this section, the namespaces used in MO are listed. These can also be found in the [pmd_mo.ttl file](https://github.com/materialdigital/application-ontologies/blob/main/microscopy_ontology_MO/pmd_mo.ttl).
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
