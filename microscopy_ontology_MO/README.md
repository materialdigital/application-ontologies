# Microscopy Ontology (MO)
This repository contains the [Microscopy Ontology (MO)](https://github.com/materialdigital/application-ontologies/blob/main/microscopy_ontology_MO/pmd_mo.ttl) and other relevant information. The MO has been developed as part of the Platform MaterialDigital [(PMD)](https://materialdigital.de/) project in collaboration with the National Institute of Standards and Technology [(NIST)](https://www.nist.gov/).
Designed as an application ontology, the MO imports and builds upon the PMD Core Ontology ([PMDco](https://github.com/materialdigital/core-ontology/tree/main)), a mid-level ontology for materials science and engineering ([more details here](https://doi.org/10.1016/j.matdes.2023.112603)), and extends the PMDco with approx. 200 terms retrieved from an NLP approach by analyzing 2 decades of [Microscopy and Microanalysis Conference](https://microscopy.org/past-m-m-meetings) proceedings. 

## Scope 
"available soon"

## Documentation
An HTML documentation of MO that was auto-generated using [Widoco tool](https://github.com/dgarijo/Widoco) implemented as an GitHub action can be found at the [gh-pages of MO](https://materialdigital.github.io/application-ontologies/mo/index-en.html) and using the MO namespace [https://w3id.org/pmd/mo](https://w3id.org/pmd/mo).

## Contribute
An open [MO HackMD document](https://hackmd.io/21tFuZTITq2draxRPbepzg) used for collaborative work on shared vocabulary / thesaurus used for [pmd_mo.ttl](https://github.com/materialdigital/application-ontologies/blob/main/microscopy_ontology_MO/pmd_mo.ttl) is available. Please feel free to contribute but highlight changes in the thesaurus.

## Publication | Citation
When using and referring to the Microscopy Ontology (MO), please cite the following publication, which provides comprehensive details and the foundational rationale behind the development of this ontology:

"available soon"

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
