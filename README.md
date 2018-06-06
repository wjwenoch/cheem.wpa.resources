- [x] add links to base KBs 
- [] literature review on AXI
- [] report on the state-of-the-art

# On explanations
## NLP-based resources
Inference-based explanations for science questions, etc. See http://cognitiveai.org/explanationbank/
The dataset COLING 2016 is a good one for understanding the details in the paper [http://cognitiveai.org/wp-content/uploads/2017/11/jansen_et_al_coling2016_whats_in_an_explanation_knowledge_inference_requirements.pdf|Paper]



# Venues for publishing/collaboration
## Conferences
|Conference|CFP|Remarks|
|----------|---|-------|
|AAAI/ACM Conference on AI, Ethics, and Society|http://www.aies-conference.com |Submission deadline: October 31st, 2017| 


# Data Resources

## Knowledge bases (KB)

### General purpose KB
|KB Name | Link | Remarks |
|--------|------|---------|
|YAGO|https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/yago/ | Manual verification, high accracy. Yago3 is open source now (https://github.com/yago-naga/yago3). 17m entities and 150m facts.|
|:BaseKB|http://basekb.com/ |Converted from Freebase with 1.3 billion facts about 40 million subjects|
|Freebase|https://developers.google.com/freebase | Project shut down, but data dump available (1.9 billion triples)|
|ConceptNet5|http://conceptnet.io/ |Multilingual. 8m nodes, 21m edges, with 1.5m nodes in English. Paper on word embeddings using ConceptNet (https://arxiv.org/pdf/1612.03975.pdf)|
|DBpedia|http://wiki.dbpedia.org/downloads-2016-04 | Multilingual. 38.3m subjects in all languages, 4.5m subjects in English.|
|Wikidata|https://www.wikidata.org |Multilingual. 34m items.|
|Webchild|https://www.mpi-inf.mpg.de/departments/databases-and-information-systems/research/yago-naga/webchild/ | 
|Babelnet|http://babelnet.org/ |Multilingual. 14m entries. Wordnet based.|
|Google KG|https://developers.google.com/knowledge-graph/ |Not great coverage/hierarchy/expressivity, but easy to access|

Note on the deprecated Freebase: some (not all) of the Freebase entities are linked to Wikidata entities, and they can identified using SPARQL queries on Wikidata as long as the Freebase identifiers are known, e.g., 
```
SELECT ?ent WHERE {
  ?ent wdt:P646 "/m/0bgvcp"
}
```
### Domain KB
|KB Name | Link | Remarks |
|--------|------|---------|
|The OBO Foundry|http://www.obofoundry.org/ | A collection of domain ontologies, incl. GO, BFO and many others. |
|Oxford ontology library|http://www.cs.ox.ac.uk/isg/ontologies/lib/ | |
|Bio-ontologies|http://bioportal.bioontology.org/ | |
|Protege ontology repo|https://protegewiki.stanford.edu/wiki/Protege_Ontology_Library#OWL_ontologies | Protege is the most popular ontology editor developed in Stanford|
|Dumontier's repo|http://dumontierlab.com/ontologies.php | Prof. Dumontier's collection of Biomedical KBs |


# References
## on Whitebox Deep Learning
Hinton's [recent paper](https://research.google.com/pubs/pub46351.html) in NIPS 2017 on "Capsules". See also his [old paper on capsules](http://www.cs.toronto.edu/~fritz/absps/transauto6.pdf)
## on XAI
### Venues
There are several workshops under main AI conferences dedicated for explanations and interpretability in machine learning. The links given are for the latest series only. 
+ Interpretable ML for Complex Systems@NIPS2016 [link](https://sites.google.com/site/nips2016interpretml/)
+ Workshop on Human Interpretability in Machine Learning (WHI)@ICML [link2](https://sites.google.com/site/2016whi/) [link2](https://2017.icml.cc/Conferences/2017/Schedule?showEvent=20)
+ IJCNN 2017 Explainability of Learning Machines [link](http://gesture.chalearn.org/ijcnn17_explainability_of_learning_machines)
+ ExaCt: Explanation-aware Computing [dblp link](http://dblp.uni-trier.de/db/conf/exact/index.html)
