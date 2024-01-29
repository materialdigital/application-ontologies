# Precipitate Geometry Ontology (PGO)

This repository comprises information on the precipitate geometry ontology (PGO) that was developed within the frame of the collaborative project 
Platform MaterialDigital (PMD): [PMD website](https://materialdigital.de/). 
It is designed as an application ontology by importing and thus making use of the mid-level PMD Core Ontology (PMDco). Hence, it can be found within this [PGO application ontology repository](https://github.com/materialdigital/application-ontologies/tree/main/precipitate_geometry_ontology_PGO) as a part of the [PMD application ontology (PMDao)](https://github.com/materialdigital/application-ontologies/tree/main) repository.

The PGO is part of the "Orowan Demonstrator" that is supposed to show the benefits of the usage of semantically structured data that were created in a typical pipeline of data generation from materials testing to RDF data in a triple store (example for semantic interoperability). As such, the PGO describes the analysis of precipitates particle sizes obtained from a typical transmission electron microscopy (TEM) process. The corresponding data obtained are referred to mechanical material characterization data to map the well-known relation of strength values obtained from tensile tests (represented by values of the yield strength Rp0.2 as obtained from classic tensile tests of metallic materials, described by the [Tensile Test Ontology (TTO)](https://github.com/materialdigital/application-ontologies/tree/main/tensile_test_ontology_TTO)) to the reciprocal values of the average distance of precipitates in accordance with the Orowan mechanism. 
Thereby, within the "Orowan Demonstrator", several ontologies are combined, one of which is the PGO.

## Namespaces
In this section, the namespaces used in PGO are listed. These can also be found in the [pmd_pgo.ttl file](https://github.com/materialdigital/application-ontologies/blob/main/precipitate_geometry_ontology_PGO/pmd_pgo.ttl).
Since PGO imports the PMDco, the PMDco namespace (https://w3id.org/pmd/co/) is used for ontological concepts.
The base of the PGO (IRI of the ontology) is https://w3id.org/pmd/pgo/. 

| Prefix | Namespace / URI                             |
|:-------|---------------------------------------------|
| :      | https://w3id.org/pmd/co/                    |
| owl    | http://www.w3.org/2002/07/owl#              |
| rdf    | http://www.w3.org/1999/02/22-rdf-syntax-ns# |
| xml    | http://www.w3.org/XML/1998/namespace        |
| xsd    | http://www.w3.org/2001/XMLSchema#           |
| rdfs   | http://www.w3.org/2000/01/rdf-schema#       |
| base   | https://w3id.org/pmd/co/                    |
