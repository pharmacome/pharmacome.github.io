## Knowledge Storage, Manipulation, and Exploration

One of the first goals of the Human Brain Pharmacome Project is to bring order
to the unstructured knowledge locked in the biomedical literature, patents,
and electronic health records.

### Storing Knowledge: Biological Expression Language

We heavily rely on Biological Expression Language (BEL) as a format for storing qualitative causal and correlative 
relations between biological entities across multiple modes and scales, with full provenance information including 
namespace references, relation provenance (citation and evidence), and biological context-specific relation metadata 
(anatomy, cell, disease etc.)

#### References

- Publication: Slater, T. (2014). [Recent advances in modeling languages for pathway maps and computable biological networks](https://doi.org/10.1016/j.drudis.2013.12.011). Drug Discovery Today, 19(2), 193–198. 
- BEL Enhancement Proposals: [https://github.com/belbio/bep](https://github.com/belbio/bep)

### Manipulating Knowledge: PyBEL

<img src="img/pybel-logo.png" alt="PyBEL Logo" height="45px" width="45px" style="float: left; margin: 5px" /> We built 
PyBEL for parsing, validating, compiling, and converting networks encoded in BEL. PyBEL comprises five main components:
(i) network data container, (ii) parser and validator, (iii) network database manager, (iv) data converter and (v) 
network visualizer.

#### References

- Publication: Hoyt, C. T., Konotopez, A., Ebeling, C. (2018). [PyBEL: a computational framework for Biological Expression Language](https://doi.org/10.1093/bioinformatics/btx660). Bioinformatics (Oxford, England), 34(4), 703–704. 
- Source Code: [https://github.com/pybel/pybel](https://github.com/pybel/pybel)
- Documentation: [http://pybel.readthedocs.io](http://pybel.readthedocs.io/)

### Exploring Knowledge: BEL Commons

<img src="img/bel-commons-logo.png" alt="BEL Commons Logo" height="45px" width="45px" style="float: left; margin: 5px" /> 
BEL Commons is an environment for curating, validating, and exploring knowledge assemblies encoded in BEL to support 
elucidating disease-specific, mechanistic insight. BEL Commons comprises five components: (i) the network uploader and 
validator, (ii) user rights and project management, (iii) the query builder, (iv) the biological network explorer and 
(iv) the analytical service.

<img src="img/bel-commons-components.png" alt="BEL Commons Components"/>

#### References

- Publication: Hoyt, C. T., Domingo-Fernández, D., & Hofmann-Apitius, M. (2018). [BEL Commons: an environment for exploration and analysis of networks encoded in Biological Expression Language](https://doi.org/10.1093/database/bay126). Database, 2018(3), 1–11.
- Web application: [https://bel-commmons.scai.fraunhofer.de](https://bel-commmons.scai.fraunhofer.de)
- Source Code: [https://github.com/bel-commons](https://github.com/bel-commons)

## Curation of Unstructured Knowledge

### BEL Curation Workflow

We developed a workflow using [git](https://git-scm.com), [GitHub](https://github.com), PyBEL, and a novel [PyBEL
extension](https://github.com/pybel/pybel-git) in order to identify and address syntactical issues in BEL documents 
in a Continuous Integration setting.

<img src="img/curation-workflow.png" alt="Curation Workflow"/>

- [Zenodo Reference](http://doi.org/10.5281/zenodo.2508180): Hoyt, C. T. (2018, December 22). pybel/pybel-git v0.0.2 (Version v0.0.2). Zenodo. http://doi.org/10.5281/zenodo.2508180
- Source Code: [https://github.com/pybel/pybel-git](https://github.com/pybel/pybel-git)

### Curation of Neurodegeneration Supporting Ontology (CONSO)

While there are several useful public terminologies useful for curation of biomedical relations, there is often the 
need to develop new controlled vocabularies, thesauri, taxonomies, and ontologies. We have maintained ours with the
ability to generate BEL namespace files, OBO files, and OWL files.

- Terminology: [https://github.com/pharmacome/terminology](https://github.com/pharmacome/terminology)

### NeuroMMSig

<img src="img/neurommsig-logo.png" alt="NeuroMMSig Logo" height="45px" width="45px" style="float: left; margin: 5px" />
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

<img src="img/enrichment-workflow.png" alt="Enrichment Workflow"/>

#### Mechanism Enrichment Server References

- Publication: Hoyt, C. T., *et al* (2019). [Re-curation and Rational Enrichment of Knowledge Graphs in Biological Expression Language](https://doi.org/10.1101/536409). BioRxiv, 536409. 
- Source Code: [https://github.com/bel-enrichment/bel-enrichment](https://github.com/bel-enrichment/bel-enrichment)
- Results: [https://github.com/bel-enrichment/results](https://github.com/bel-enrichment/results)

### Topic-Specific Manual Curation

We have prioritized manual curation of the highest granularity for new content related to the human Tau protein, 
nicotoinic receptor biology, and proteostasis. They can be downloaded and handled with PyBEL (or other BEL tools) using
 the link below.

- Results: [https://github.com/pharmacome/knowledge](https://github.com/pharmacome/knowledge])

### TauBase

We've generated a dynamic web application for exploring the content curated during this project that can be found
at [https://github.com/pharmacome/taubase](https://github.com/pharmacome/taubase]). It will be deployed publicly soon.

## Acquisition and Transformation of of Unstructured Knowledge

### Bio2BEL

<img src="img/bio2bel-logo.png" alt="Bio2BEL Logo" height="39px" width="45px" style="float: left; margin: 5px" /> 
BEL is well-suited as an biomedical knowledge integration standard as it has precise semantics and is extensible. We
generated several reusable packages for converting and harmonizing databases across modes and scales in BEL.

<img src="img/bio2bel-components.png" alt="Bio2BEL Components"/>

#### References

- Source Code: [https://github.com/bio2bel](https://github.com/bio2bel)

### ComPath

<img src="img/compath-logo.png" alt="ComPath Logo" height="45px" width="45px" style="float: left; margin: 5px" /> 
We curated mappings between three major pathway databases (KEGG, Reactome, and WikiPathways) and MSigDB to identify
their overlapping entries.

#### References

- Publication: Domingo-Fernandez, D., *et al*. (2018). [ComPath: an ecosystem for exploring, analyzing, and curating mappings across pathway databases](https://doi.org/10.1038/s41540-018-0078-8). Npj Systems Biology and Applications, 5(1), 3.
- Web Application: [https://compath.scai.fraunhofer.de](https://compath.scai.fraunhofer.de)
- Source Code: [https://github.com/ComPath/ComPath](https://github.com/ComPath/ComPath)

### PathMe

<img src="img/pathme-logo.png" alt="PathMe Logo" height="45px" width="45px" style="float: left; margin: 5px" />
We harmonized and extracted pathway knowledge from three major pathway databases: KEGG, Reactome, and WikiPathways
in order to make comparisons about their coverage and to generate consensus pathways (by using ComPath) for downstream
applications, such as with Signalling Pathway Impact Analysis (SPIA). 

#### References

- Publication: Domingo-Fernandez, D., *et al.* (2018). [PathMe: Merging and exploring mechanistic pathway knowledge](http://biorxiv.org/content/early/2018/10/24/451625.abstract). bioRxiv, 451625.
- Web Application: [https://pathme.scai.fraunhofer.de](https://pathme.scai.fraunhofer.de)
- Source Code: [https://github.com/pathwaymerger/pathme](https://github.com/pathwaymerger/pathme)

## Analytical Approaches

### Comparative Mechanism Enrichment

We proposed an explanation for the cross-indication effects of Carbamazepine towards epilepsy and Alzheimer's disease
by using the NeuroMMSig mechanism enrichment server to identify overlapping mechanisms with its experimentally measured 
and computationally predicted targets.

#### References

- Publication: Hoyt, C. T. and Domingo-Fernández, D., *et al.* (2018). [A systematic approach for identifying shared mechanisms in epilepsy and its comorbidities](https://doi.org/10.1093/database/bay050). Database, 2018(1). 

### Target Prioritization with Network Representation Learning

We used GAT2VEC to generate random walk-based node embeddings for protein-protein interaction (PPI) networks annotated 
with disease-specific differential gene expression profiles from GEO, ArrayExpress, and other sources. Following
the prediction and evaluation pipeline from Emig, *et al.* (2013), we built simple generalized linear models using 
annotations from OpenTargets as a training set and generated rankings for all targets.

#### References

- Publication: Muslu, Ö., Hoyt, C. T., Hofmann-Apitius, M., & Fröhlich, H. (2019). [GuiltyTargets: Prioritization of Novel Therapeutic Targets with Deep Network Representation Learning](https://doi.org/10.1101/521161). BioRxiv, 1–14. 
- See Also: Emig, D., *et al.* (2013). [Drug Target Prediction and Repositioning Using an Integrated Network-Based Approach](https://doi.org/10.1371/journal.pone.0060618). PLoS ONE, 8(4).
- Source Code: [https://github.com/guiltytargets](https://github.com/guiltytargets)

### Link Prediction with Network Representation Learning

We generated two network representation learning (NRL) libraries: [one](https://github.com/cthoyt/nrl) for random 
walk-based NRL and [another](https://github.com/smartDataAnalytics/pykeen) for semantic translations models and
neural network models.

#### References

- Publication: Ali, M., Hoyt, C. T., Domingo-Fernández, D., Lehmann, J., & Jabeen, H. (2018). [BioKEEN: A library for learning and evaluating biological knowledge graph embeddings](https://doi.org/10.1101/475202), 1–5. 
- Source Code (NRL): [https://github.com/cthoyt/nrl](https://github.com/cthoyt/nrl)
- Source Code (PyKEEN): [https://github.com/smartDataAnalytics/pykeen](https://github.com/smartDataAnalytics/pykeen)
- Source Code (BioKEEN): [https://github.com/smartDataAnalytics/biokeen](https://github.com/smartDataAnalytics/biokeen)

## Funding

We're funded by the Fraunhofer Society's MAVO program as a joint undertaking between 
[Fraunhofer SCAI](https://www.scai.fraunhofer.de/), [Fraunhofer IAIS](https://www.iais.fraunhofer.de), 
and [Fraunhofer IME](https://www.ime.fraunhofer.de/). Also, see our [blog](https://pharmacome.scai.fraunhofer.de/).
