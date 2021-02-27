## Intraoral radiograph anatomical region classification using neural networks.

This repository contains the code used in the following paper [full text link]:\
[**Kyventidis, N., Angelopoulos, C. Intraoral radiograph anatomical region classification using neural networks. Int J CARS (2021).**](https://rdcu.be/cfNeV) [**DOI:10.1007/s11548-021-02321-4**](https://doi.org/10.1007/s11548-021-02321-4)

The anatomic class relative to the depicted anatomy of digital intraoral (dental) radiographs has to be manually preselected during exposure or manually added later. Since at least half a billion intraoral radiographs are produced every year, automating this task could provide substantial benefits. A novel methodology enabling automatic classification by employing neural networks is presented in the paper.


You can use the code in this repository to train and validate your own classifiers. Please inform us in case you reproduce the results of this experiment with your own dataset.


**Please note:**
*Code for this project is currently being migrated to TensorFlow 2 and will be posted shortly.*

Some notable changes from the original article:

- migrated to TensorFlow 2.
- sklearn's AUC metric has been replaced with tf.keras AUC metric.
- class weights are now calculated with sklearn's "class_weight" function.


### Setup
Coming soon

### Guide
Comming soon


### Cite as:

If you find this article useful in your own research, please cite as (bibtex entry provided below):

@article{\
	title = {Intraoral radiograph anatomical region classification using neural networks},\
	issn = {1861-6429},\
	url = {https://doi.org/10.1007/s11548-021-02321-4}, \
	doi = {10.1007/s11548-021-02321-4},\
	abstract = {Dental radiography represents 13\% of all radiological diagnostic imaging. Eliminating the need for manual classification of digital intraoral radiographs could be especially impactful in terms of time savings and metadata quality. However, automating the task can be challenging due to the limited variation and possible overlap of the depicted anatomy. This study attempted to use neural networks to automate the classification of anatomical regions in intraoral radiographs among 22 unique anatomical classes.},\
	journal = {International Journal of Computer Assisted Radiology and Surgery},\
	author = {Kyventidis, Nikolaos and Angelopoulos, Christos},\
	month = feb,\
	year = {2021}\
}





