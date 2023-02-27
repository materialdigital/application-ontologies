# Tensile Test Ontology (TTO)

This repository comprises the tensile test ontology (TTO) that was developed within the frame of the joint project 
Platform MaterialDigital (PMD): [PMD website](https://materialdigital.de/). 
It is therefore classified as PMD application ontology (PMDao).

<!-- TOC -->
1. [Abstract](#Abstract)
2. [Documents | Links](#Documents-|-Links)
3. [Documentation](#Documentation)
   1. [Ontology Development Steps](#Ontology-Development-Steps)
   2. [Design Principles | Decision log](#Design-Principles-|-Decision-log)
      1. [Fundamentals](#Fundamentals)
      2. [Case decisions | Specific issues](#Case-decisions-|-Specific-issues)
      3. [Namespaces](#Namespaces)
<!-- TOC -->

## Abstract
This document is supposed to provide general information on the development of an 
ontology in the field of materials sciences and engineering (MSE) that was 
realized within [PMD](https://materialdigital.de) as a first best practice example. 
Accordingly, it is supposed to give specifically documentation on the development of the tensile test ontology (TTO). 
Hence, besides its informative character, this document may allow the 
developers to explain, register and secure distinct decisions made during 
the ontology development process. As such, it serves as a kind of log book.

The material's characterization process of the tensile test on 
metallic materials at room temperature (henceforth simply referred 
to as 'tensile test') was semantically described in accordance with the 
standard DIN EN ISO 6892-1:2019-11. In particular, terms, definitions and 
symbols given in the standard are used in the TTO. Furthermore, a 'preferable data structure' (cf. section [Documents | Links](#Documents-|-Links)) in terms of the categorization
of typical data resulting from a tensile test was developed in an ad-hoc group formed by experts of the DIN standardization
committee being in charge of the corresponding DIN EN ISO 6892-1. This data structure depicts the MSE experts' view on how tensile
test data is supposed to be categorized and, in particular, which data may be recorded and provided by testers 
to obtain a comprehensive tensile test dataset.


The resulting [TTO](https://github.com/materialdigital/application-ontologies/blob/main/tensile_test_ontology_TTO/pmdao_TTO.ttl) is supposed to be publicly available on the 
[PMD website](https://materialdigital.de/download/) (download section, available after free registration), this [PMD GitHub repository](https://github.com/materialdigital/application-ontologies/tree/main/tensile_test_ontology_TTO) 
and on [MatPortal.org](https://matportal.org/ontologies). 

The TTO was strongly designed on the basis of the PMD core ontology ([PMDco](https://github.com/materialdigital/core-ontology)). 
Accordingly, classic PMDco concepts are re-used and concepts included due to
the consideration of the tensile test are always connected to PMDco concepts.
Moreover, PMDco is connected to other (higher-level) ontologies (cf. section [Documents | Links](#Documents-|-Links)).
Therefore, a consideration of the PMDco and its documentation is recommended.

*Furthermore, there is an earlier version of the TTO that was developed as first
approach to provide an example for the creation of an application ontology.
The result of this development is also given in this repository in a separate
branch ([TTO_0.1](https://github.com/materialdigital/application-ontologies/tree/main/tensile_test_ontology_TTO)).* 

## Documents | Links
In this section, some documents and tools are listed (and linked, if applicable) that 
supported the ontology creation or provide some additional information.

+ [Repository of TTO](https://github.com/materialdigital/application-ontologies/tree/main/tensile_test_ontology_TTO) | Files will be stored here, e.g., TTL file of TTO or exemplary RDF files
+ [Tensile Test Ontology (TTO)](https://github.com/materialdigital/application-ontologies/blob/main/tensile_test_ontology_TTO/pmdao_TTO.ttl) | TTL file of the TTO in this repository
+ [Standard ISO 6892-1:2019-11](https://www.beuth.de/de/norm/iso-6892-1/316885984) | The ISO standard the TTO development is based on
+ [Visualization of preferable tensile test data structure](https://github.com/materialdigital/application-ontologies/blob/main/tensile_test_ontology_TTO/Tensile_Test_Data_Structure_DIN_ad-hoc.pdf) | Visualization of a preferable tensile test data structure, which is the result of an ad-hoc group of the DIN EN ISO 6892-1 standardization committee; basis for TTO development
+ [PMD core ontology (PMDco)](https://github.com/materialdigital/core-ontology) | The mid-level ontology in the field of materials sciences and engineering (MSE) the TTO is based on
+ [Ontopanel tool](https://yuechenbam.github.io/src/main/webapp/index.html) | A tool created for domain experts based on [diagrams.net](https://www.diagrams.net/) that facilitates visual ontology development and mapping for FAIR data sharing in materials testing (more information in open access [scientific paper](https://link.springer.com/article/10.1007/s40192-022-00279-y))
+ [Protégé tool](https://protege.stanford.edu/) | A tool used for the creation of ontologies; especially, annotations and relations were included in the ontology by applying the Protégé tool

Furthermore, other (higher-level) ontologies are used in TTO since their 
concepts are partly also included in PMDco. Such are
+ Basic Formal Ontology ([BFO](https://basic-formal-ontology.org/)),
+ The PROV Ontology ([PROV-O](https://www.w3.org/TR/prov-o/)),
+ European Materials Modelling Ontology ([EMMO](https://github.com/emmo-repo/EMMO)),
+ Chemical Entities of Biological Interest Ontology ([ChEBI](https://www.ebi.ac.uk/chebi/)). 



## Documentation
This section provides information on the TTO development process and fundamental
design principles used in TTO. Some basic design principles are already given
in the PMDco the TTO is based on.

### Ontology Development Steps
During the development of TTO, the following steps were taken:
1. Usage of all necessary and supporting information, e.g., ISO standard(s) and preferable data structure(s) created therefrom
2. Creation of concepts and plausible relations (T-Box) between them on a visual basis using Ontopanel tool
3. Conversion into OWL / TTL by using the built-in conversion plugin of Ontopanel
4. Annotation and curation of concepts using Protégé tool, including definitions of concepts, classes, object properties, entities using annotation functionality and adding relations between concepts
5. Verification by reasoning in Protégé

Since the development of ontologies is an iterative process that might 
include both, the possibility and the demand to adjust and extend the 
ontology, the development steps presented above are also iterative and were 
used in repeated sequence. In particular, steps 2 and 3 were repeated 
numerously after findings in step 5 and also possible changes concerning 
implemented content. Likewise, steps 4 and 5 were repeatedly taken when new 
relations between concepts were introduced.

### Design Principles | Decision log
In this section, **design principles** used to model the TTO and, 
especially, underlying modelling decisions are logged and explained with 
a focus on modelling goals.

#### Fundamentals
Some basic ideas and conceptual approaches that were kept in mind when creating TTO are given in note form (most ideas also affected PMDco creation and are therefore also realized in PMDco):
+ include many classes that allow interconnection / interoperability / reuse
+ object properties defined are condensed to a lower number to reach clarity
+ re-usage of known and well-established concepts / schema is preferred (usage of higher-level ontologies), such as in the field of datatype definitions
+ including labels using *rdfs:label*, *skos:preflabel*, *skos:altlabel* and definitions as *skos:definition* (using Protégé tool) for human readability
+ if applicable, usage examples are provided via *skos:example*
+ MSE (domain) knowledge is included in class definitions - by including human-readable definitions given in natural-language as well as by implementing class relations
+ human-readable identifiers for better understanding - labels as well as class / object property designation lead to enhanced query-ability 
+ PMDco (core ontology = mid-level ontology) is used as basis for ontology development, i.e. basic classes and properties, which are partly related to higher-level ontologies, are frequently used

#### Case decisions | Specific issues

| Aim / modelling goal                                                                                                                                                        | Decision / modelling approach                                                                                                       | Remarks / Explanation                                                                                                                                                                                                                                                                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Integration of generic terms and definitions from the field of MSE                                                                                                          | Usage of higher-level ontologies (e.g. EMMO), if possible; add own definitions.                                                     | Since basic MSE concepts are to be included, concepts already given in other ontologies (e.g. in EMMO) are used to avoid doubled work. If there are no concepts that fit the specific need, such are simply created.                                                                                                                     |
| Include concepts of (characteristic) parameters to the characterization method description. Q: Where to put such parameters conceptually - to TT process or the test piece? | Due to the general modelling approach using the mid-level ontology PMDco, such parameters are connected as 'output' to the process. | In general, this modelling is process-centered as the ontology is supposed to focus the tensile test process and respective data originating therefrom. Therefore, especially, characteristic values are semantically connected to the process. Data distinctly referring to the test piece are accordingly connected to the test piece. |
| Include expressivity for the description of the material used, e.g., 'steel'.                                                                                               | The possibility to name the material used was inherited from the PMDco using the class *'MaterialDesignation'*                      | The material tested in a tensile test has to be named, for sure. This is possible using the *'MaterialDesignation'* class. Some more expressivity can be included by using the classes given by PMDco to describe chemical compositions.                                                                                                 |


#### Namespaces
In this section, the namespaces used in TTO are listed. These can also be found in the [pmdao_TTO.ttl file](https://github.com/materialdigital/application-ontologies/blob/main/tensile_test_ontology_TTO/pmdao_TTO.ttl). By definition,
https:// is commonly used for namespaces.

| Prefix | Namespace / URI                              |
|:-------|----------------------------------------------|
| :      | https://material-digital.de/pmdco/           |
| owl    | https://www.w3.org/2002/07/owl#              |
| rdf    | https://www.w3.org/1999/02/22-rdf-syntax-ns# |
| sdo    | https://schema.org/                          |
| xml    | https://www.w3.org/XML/1998/namespace        |
| xsd    | https://www.w3.org/2001/XMLSchema#           |
| rdfs   | https://www.w3.org/2000/01/rdf-schema#       |
| base   | https://material-digital.de/pmdao/tto        |