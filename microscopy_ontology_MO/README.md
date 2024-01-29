# Microscopy Ontology (MO)

This repository comprises information on and file related to the microscopy ontology (MO) that was developed within the frame of the collaborative project 
Platform MaterialDigital (PMD): [PMD website](https://materialdigital.de/). 
It is designed as an application ontology by importing and thus making use of the mid-level PMD Core Ontology ([PMDco](https://github.com/materialdigital/core-ontology/tree/main)). Hence, it can be found within this [MO application ontology repository](https://github.com/materialdigital/application-ontologies/tree/main/microscopy_ontology_MO) as a part of the [PMD application ontology (PMDao)](https://github.com/materialdigital/application-ontologies/tree/main) repository.

The PGO is part of the "Orowan Demonstrator" that is supposed to show the benefits of the usage of semantically structured data that were created in a typical pipeline of data generation from materials testing to RDF data in a triple store (example for semantic interoperability). As such, the PGO describes the analysis of precipitates particle sizes obtained from a typical transmission electron microscopy (TEM) process. The corresponding data obtained are referred to mechanical material characterization data to map the well-known relation of strength values obtained from tensile tests (represented by values of the yield strength Rp0.2 as obtained from classic tensile tests of metallic materials, described by the [Tensile Test Ontology (TTO)](https://github.com/materialdigital/application-ontologies/tree/main/tensile_test_ontology_TTO)) to the reciprocal values of the average distance of precipitates in accordance with the Orowan mechanism. 
Thereby, within the "Orowan Demonstrator", several ontologies are combined, one of which is the PGO.

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
