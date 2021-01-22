---
title: stardist
layout: page
---

- *Contributor(s)*: Uwe Schmidt (@uschmidt83), Martin Weigert (@maweigert)
- *References*: [Github](https://github.com/mpicbg-csbd/stardist), [Publications](https://github.com/mpicbg-csbd/stardist#how-to-cite)

## Purpose

> Describe the problem you are trying to solve by packaging your tool as a napari plugin in 1-2 sentences.
I should be able to read this alone and communicate the value to someone else.

This plugin will allow users to segment round objects (such as cell nuclei) in 2D microscopy images by providing a prediction interface for pretrained/custom trained *stardist* networks

## Goals
> What would you like to accomplish during the Alfa Cohort collaboration?

1. Allow biologists to apply pre-trained stardist models to segment nuclei in 2D images
2. Apply custom trained stardist model in 2D
3. [stretch] the same for 3D models

### Non-goals
> Are there any possible goals that are explicitly out of scope for the Alfa Cohort?

1. Allowing user to perform model training from within napari

## Scope

### Key Flows

> Show what the end-to-end experience will be for biologists.

A biologist will be able to
1. Load their own imaging data
  - One image at a time?
  - How to handle timelapse?
2. Select a custom or pre-trained stardist model
  - Ideal: Give user visibility into imaging modality relevant to a model
3. Set or adjust parameters & normalize data
4. Apply the model
5. View results (masks / label image)
6. Aggregation of results. Export labeled images.


## Plan

### Milestones

> Status: To Do 📝, In Progress 🏗, In Review 🔎, Done ✅

| TARGET DATE 	| MILESTONE                        	| DESCRIPTION                                                                                                                	| STATUS 	|
|-------------	|----------------------------------	|----------------------------------------------------------------------------------------------------------------------------	|--------	|
|             	| Create deployment infrastructure 	| Create native stardist python wheels to allow installation into napari environment without compilation                     	|    📝   	|
|             	| Simple stardist UX               	| Create a UX for single timepoint/single channel application of pretrained stardist models on already opened napari images  	|    📝   	|
|             	| Final stardist UX                	| Add timelapse/multichannel modality, parameter adjustment, results export                                                  	|    📝   	|
| 2021-04-28  	| Demo day                         	| Demo final plugin                                                                                                          	|    📝   	|
