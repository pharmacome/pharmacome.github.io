## Knowledge Storate, Manipulation, and Exploration

One of the first goals of the Human Brain Pharmacome Project is to bring order
to the unstructured knowledge locked in the biomedical literature, patents,
and electronic health records.

### Storing Knowledge: Biological Expression Language

We heavily rely on Biological Expression Language (BEL) as a format for storing qualitative causal and correlative relations between biological entities across multiple modes and scales, with full provenance information including name- space references, relation provenance (citation and evidence), and biological context-specific relation metadata (anatomy, cell, disease etc.)

#### References

- Publication: Slater, T. (2014). [Recent advances in modeling languages for pathway maps and computable biological networks](https://doi.org/10.1016/j.drudis.2013.12.011). Drug Discovery Today, 19(2), 193–198. 
- BEL Enhancement Proposals: [https://github.com/belbio/bep](https://github.com/belbio/bep)

### Manipulating Knowledge: PyBEL

<img src="img/pybel-logo.png" alt="PyBEL Logo" height="45px" width="45px" style="float: left; margin: 15px" /> We built PyBEL for parsing, validating, compiling, and converting networks encoded in BEL.

#### References

- Publication: Hoyt, C. T., Konotopez, A., Ebeling, C. (2018). [PyBEL: a computational framework for Biological Expression Language](https://doi.org/10.1093/bioinformatics/btx660). Bioinformatics (Oxford, England), 34(4), 703–704. 
- Source Code: [https://github.com/pybel/pybel](https://github.com/pybel/pybel)
- Documentation: [http://pybel.readthedocs.io](http://pybel.readthedocs.io/)

### Exploring Knowledge: BEL Commons

<img src="img/bel-commons-logo.png" alt="BEL Commons Logo" height="45px" width="45px" style="float: left; margin: 15px" /> BEL Commons is an environment for curating, validating, and exploring knowledge assemblies encoded in BEL to support 
elucidating disease-specific, mechanistic insight.

<img src="img/bel-commons-components.png" alt="BEL Commons Components" width="424" height="283"/>

#### References

- Publication: Hoyt, C. T., Domingo-Fernández, D., & Hofmann-Apitius, M. (2018). [BEL Commons: an environment for exploration and analysis of networks encoded in Biological Expression Language](https://doi.org/10.1093/database/bay126). Database, 2018(3), 1–11.
- Web application: [https://bel-commmons.scai.fraunhofer.de](https://bel-commmons.scai.fraunhofer.de)
- Source Code: [https://github.com/bel-commons](https://github.com/bel-commons)

## Knowledge Acquisition, Transformation, and Curation

### BEL Curation Workflow

<img src="img/curation-workflow.png" alt="Curation Workflow" width="424" height="424"/>

- [Zenodo Reference](http://doi.org/10.5281/zenodo.2508180): Hoyt, C. T. (2018, December 22). pybel/pybel-git v0.0.2 (Version v0.0.2). Zenodo. http://doi.org/10.5281/zenodo.2508180
- Source Code: [https://github.com/pybel/pybel-git](https://github.com/pybel/pybel-git)

### Curation of Neurodegeneration Supporting Ontology (CONSO)

While there are several useful public terminologies useful for curation of biomedical relations, there is often the 
need to develop new controlled vocabularies, thesauri, taxonomies, and ontologies. We have maintained ours with the
ability to generate BEL namespace files, OBO files, and OWL files.

- Terminology: [https://github.com/pharmacome/terminology](https://github.com/pharmacome/terminology)

### NeuroMMSig

Multimodal mechanistic signatures for neurodegenerative diseases (NeuroMMSig) consists of three parts: a taxonomy
of candidate pathophysiological mechanisms in three neurodegenerative diseases (i.e., Alzheimer's disease, Parkinson's 
disease, and epilepsy), disease-specific mechanistic models of each, and a web server implementing
a novel mechanism enrichment algorithm.

#### Disease Mechanism Inventory References

- Terminology: [https://github.com/neurommsig/neurommsig-terminology](https://github.com/neurommsig/neurommsig-terminology)
- Disease Mechanisms: [https://github.com/neurommsig/neurommsig-knowledge](https://github.com/neurommsig/neurommsig-knowledge)

#### Mechanism Enrichment Server References

- Publication: Domingo-Fernández, D., *et al.* (2017). [Multimodal mechanistic signatures for neurodegenerative diseases (NeuroMMSig): A web server for mechanism enrichment](https://doi.org/10.1093/bioinformatics/btx399). Bioinformatics, 33(22), 3679–3681. 
- Web application: [https://neurommsig.fraunhofer.de](https://neurommsig.fraunhofer.de)

### Rational Enrichment of NeuroMMSig

<img src="img/enrichment-workflow.png" alt="Enrichment Workflow" width="424" height="424"/>

#### Mechanism Enrichment Server References

- Publication: Hoyt, C. T., *et al* (2019). [Re-curation and Rational Enrichment of Knowledge Graphs in Biological Expression Language](https://doi.org/10.1101/536409). BioRxiv, 536409. 
- Source Code: [https://github.com/bel-enrichment/bel-enrichment](https://github.com/bel-enrichment/bel-enrichment)
- Results: [https://github.com/bel-enrichment/results](https://github.com/bel-enrichment/results)

### Topic-Specific Manual Curation

We have prioritized manual curation of the highest granularity for new content related to the human Tau protein, 
nicotoinic receptor biology, and proteostasis. They can be downloaded and handled with PyBEL (or other BEL tools) using
 the link below.

- Results: [https://github.com/pharmacome/knowledge](https://github.com/pharmacome/knowledge])

### Bio2BEL

- Source Code: [https://github.com/bio2bel](https://github.com/bio2bel)

## Analytical Approaches

### Comparative Mechanism Enrichment

#### References

- Publication: Hoyt, C. T. and Domingo-Fernández, D., *et al.* (2018). [A systematic approach for identifying shared mechanisms in epilepsy and its comorbidities](https://doi.org/10.1093/database/bay050). Database, 2018(1). 

### Clustering with Network Representation Learning

#### References

- Publication: Muslu, Ö., Hoyt, C. T., Hofmann-Apitius, M., & Fröhlich, H. (2019). [GuiltyTargets: Prioritization of Novel Therapeutic Targets with Deep Network Representation Learning](https://doi.org/10.1101/521161). BioRxiv, 1–14. 
- Source Code: [https://github.com/guiltytargets](https://github.com/guiltytargets)

### Link Prediction with Network Representation Learning

#### References

- Publication: Ali, M., Hoyt, C. T., Domingo-Fernández, D., Lehmann, J., & Jabeen, H. (2018). [BioKEEN: A library for learning and evaluating biological knowledge graph embeddings](https://doi.org/10.1101/475202), 1–5. 
- Source Code (PyKEEN): [https://github.com/smartDataAnalytics/pykeen](https://github.com/smartDataAnalytics/pykeen)
- Source Code (BioKEEN): [https://github.com/smartDataAnalytics/biokeen](https://github.com/smartDataAnalytics/biokeen)
