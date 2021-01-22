---
title: <Project Name>
layout: page
---

- *Contributor(s)*: Adam Tyson (@adamltyson)
- *References*: [Project Site](https://cellfinder.info/), [Github](https://github.com/brainglobe/cellfinder), [Documentation](https://docs.brainglobe.info/cellfinder/introduction), [Publication](https://www.biorxiv.org/content/10.1101/2020.10.21.348771v1)

## Purpose

> Describe the problem you are trying to solve by packaging your tool as a napari plugin in 1-2 sentences.
I should be able to read this alone and communicate the value to someone else.

### Why does this matter to biologists?

cellfinder can quickly detect cells in large datasets, but it is currently limited to command-line use, and is optimised for whole-brain microscopy. Packaging in napari will remove barriers for users and allow it to be used in more general workflows.

### Why does this matter to you and your professional goals and responsibilities?

Packaging in napari will increase adoption of the tool, and hopefully help future-proof it, reducing the maintenance load long-term.

## Goals
> What would you like to accomplish during the Alfa Cohort collaboration?

1. Isolate the cell detection portion of cellfinder and implement as a napari plugin
2. Implement a user-friendly GUI for curation of cell detection results, and retraining the classification network.
3. Identify a second biological application that the algorithm is relevant to (non-brain but similar size - 0.5cc)

### Non-goals
> Are there any possible goals that are explicitly out of scope for the Alfa Cohort?

1. Implementation of full brainglobe suite as napari plugin. To do at a later date

## Scope

### Key Features

During the Alfa Cohort
1. cell detection algorithm of cellfinder available as a modular Python package
2. Algorithm implemented as a napari extension to work with all supported raw data formats
3. Data curation/training interface implemented within napari extension

Future considerations
1. User interaction: Live updates during algorithm execution
2. Algorithm: add support for 2D data, not just 3D
3. Algorithm: extend support for N channels instead of strictly 2
4. Algorithm: extend support for N output classes (i.e. not just cell detection, but cell-type classification).


### Key Flows

> Show what the end-to-end experience will be for biologists.

A biologist will be able to
1. Apply cellfinder algorithm to data loaded in napari
2. Review results to curate correct and incorrect results (and generate training data)
3. Save outputs for further analysis
4. Train classification model and save trained model for offline analysis

## Plan

### Milestones

> Status: To Do 📝, In Progress 🏗, In Review 🔎, Done ✅

| TARGET DATE 	| MILESTONE            	| DESCRIPTION                                                               	| STATUS 	|
|-------------	|----------------------	|---------------------------------------------------------------------------	|--------	|
| 2020-02-01  	| Isolated environment 	| Algorithm running isolated from brainglobe environment                    	|    📝   	|
| 2020-03-01  	| Napari integration   	| Algorithm running on napari image layers (rather than only tiffs on disk) 	|    📝   	|
| 2020-04-01  	| Retraining           	| Classification model able to be retrained within napari                   	|    📝   	|
| 2020-04-15  	| Application          	| Use on >1 biological application                                          	|    📝   	|
| 2020-04-28  	| Demo day             	| Demo final cellfinder plugin                                              	|    📝   	|
