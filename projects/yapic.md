---
title: YAPiC
layout: page
---

- *Contributor(s)*: Pranjal Dhole (@pranjaldhole), Eugenio Fava, Christoph Moehl (@cmohl2013)
- *References*: [Project Site](https://yapic.github.io/yapic/), [Github](https://github.com/yapic/yapic)

## Purpose

> Describe the problem you are trying to solve by packaging your tool as a napari plugin in 1-2 sentences.
I should be able to read this alone and communicate the value to someone else.

### Why does this matter to biologists?

- By integrating YAPiC with Napari we provide a user-friendly workflow to train and apply U-Net based custom pixel classifiers to multidimensional image data of arbitrary size.

### Why does this matter to you and your professional goals and responsibilities?

- By integrating YAPiC with napari we expect to increase the number of YAPiC users.
- It will increase visibility of YAPiC.
- YAPiC will become more user-friendly.
- We see great potential in napari, also for the specific applications in our institute, e.g. high content screening. We hope to contribute to the development of napari in order to use it effectively in the field of drug discovery as well.

## Goals
> What would you like to accomplish during the Alfa Cohort collaboration?

1. Allow YAPiC users to label data in napari
2. Allow YAPiC users to apply a trained model for automated pixel prediction in napari and to observe the results.

### Non-goals
> Are there any possible goals that are explicitly out of scope for the Alfa Cohort?

1. Allow users to perform YAPiC training directly from napari

## Scope

### Key Flows

> Show what the end-to-end experience will be for biologists.

A biologist will be able to
1. Open Napari and import a set of multidimensional images, serving as a training data set.
2. Define a set of label classes.
3. Label pixels of the training data set to assign them to one of the label classes. Labelling can be sparse, i.e. it is not required to label all pixels of the training images.
4. Save pixel and label data in a container file format provided by Napari.
5. Transfer the data file to a linux system with appropriate GPU hardware. This may be a workstation or a GPU cluster.
run a training with the YAPiC command line tool. YAPiC reads pixels and labels from the napari data file. YAPiC saves the trained model as Keras hdf5 container.
6. Opens Napari and imports a set of images.
7. Open the Keras model file and apply the model to the image set.
8. For each output class of the model, a new pixel channel is added to the image set. The pixel intensities reflect the class probability (the classifier output).


## Plan

### Milestones

> Status: To Do 📝, In Progress 🏗, In Review 🔎, Done ✅

| TARGET DATE 	| MILESTONE                                     	| DESCRIPTION                                                                                                                                     	| STATUS       	|
|-------------	|-----------------------------------------------	|-------------------------------------------------------------------------------------------------------------------------------------------------	|--------------	|
| 15/02/2021  	| Napari-label file                             	| Portable file that contains information regarding image set and marked labels.                                                                  	|    📝 (CZI)   	|
| 15/03/2021  	| Implementation of Classes                     	| Implementation of classes within YAPiC repos such that napari-file can be used for loading train/test sets for supervised pixel classification. 	|   📝 (DZNE)   	|
| 15/03/2021  	| API interface                                 	| High-level API with documentation such that Keras model can be loaded in napari such that pixel class prediction is made on unlabelled data.    	|    📝 (CZI)   	|
| 07/04/2021  	| Development of YAPiC plugin with provided API 	| Writing up the high-level plugin with the help of provided documentation.                                                                       	|   📝 (DZNE)   	|
| 25/04/2021  	| Testing-plugin with few datasets              	| Testing the developed Plugin on databases of different sizes and formats.                                                                       	| 📝 (DZNE+CZI) 	|
| 2021-04-28  	| Demo day                                      	| Demo final plugin                                                                                                                               	|       📝      	|
