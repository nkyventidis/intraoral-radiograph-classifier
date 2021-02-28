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
We suggest using an Anaconda Python 3.8.5 environment.
Our code has been tested with:
- tensorflow 2.4.0
- numpy 1.19.2
- pandas 1.1.3
- scikit-image 0.17.2
- scikit-learn 0.23.2
- bokeh 2.2.3
- matplotlib 3.3.1


### Guide
You can train your own intraoral radiograph classifiers by providing your own dataset. All images must be placed inside a root folder and split in 'train', 'validation' and (optionally) 'test' subfolders, as well as subfolders for every class. For example:

root_folder/\
...train/\
......LBW/\
.........a_image_1.jpg\
.........a_image_2.jpg\
......11-12/\
.........b_image_1.jpg\
.........b_image_2.jpg\
etc.

The code can handle an arbitrary number of classes. We suggest using the classification described in our paper, or alternatively the one suggested by the JSOMR in the [DICOM standard](https://dicom.nema.org/medical/dicom/2019b/output/pdf/part17.pdf).

Run the following command to commence your experiment:\
```
python intraoral_classifier.py IO-classifier
```

Note that our code can also train a general purpose classifier if provided with alternate input images. For more information refer to the source itself.

### Cite as:

If you find this article/repository useful in your own research, please cite us (bibtex entry provided below):

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





