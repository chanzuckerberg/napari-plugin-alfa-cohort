---
title: Allen Cell Segmenter
layout: page
---

- *Contributor(s)*: Jianxu Chen (@jxchen01), Benjamin Morris (@benjijamorris)
- *References*: [Project Site](https://www.allencell.org/segmenter.html), [Github](https://github.com/AllenCell/aics-segmentation), [Publication](https://www.biorxiv.org/content/10.1101/491035v2), [Support](https://forum.allencell.org/c/software-code/segmenter/16)

## Purpose

> Describe the problem you are trying to solve by packaging your tool as a napari plugin in 1-2 sentences.
I should be able to read this alone and communicate the value to someone else.

### Why does this matter to biologists?

### Why does this matter to you and your professional goals and responsibilities?

## Goals
> What would you like to accomplish during the Alfa Cohort collaboration?

1. Make “lookup table” of segmentation algorithms available. Load workflow & tweak parameters based on instant feedback from the viewer. Target audience: Anyone
2. [Stretch] For more advanced user who knows a bit about the algorithms, they have the freedom to manipulate the workflow. Freedom to use modules.
3. [Ultra Stretch] Integrating with ML model. Curation of pass/fail (not painting). Use case: different areas of image may need different algorithm. Then a set of training data is ready for training.


### Non-goals
> Are there any possible goals that are explicitly out of scope for the Alfa Cohort?

1. Not going to support 2D at this time

## Scope

### Key Flows

> Show what the end-to-end experience will be for biologists.

A biologist will be able to
1. Load some 3D data
2. Select a workflow which is tuned for a particular cell structure
3. Apply the workflow and see results
4. Tweak parameters for each step in the workflow based on instant feedback from the viewer
5. Save the parameters + workflow
6. Apply the parameters + workflow to larger set of images
7. Analyze the results to extract statistics of cell structures

[Stretch] A biologist will be able to
1. Load and apply a workflow (above 1 through 4)
2. View the steps that the workflow implements
3. Add or remove steps and adjust parameters
4. Then do 5 through 7 above


## Plan

### Milestones

> Status: To Do 📝, In Progress 🏗, In Review 🔎, Done ✅

| Target Date 	| Milestone 	| Description       	| Status 	|
|-------------	|-----------	|-------------------	|--------	|
|             	|           	|                   	|        	|
|             	|           	|                   	|        	|
| 2020-04-28  	| Demo day  	| Demo final plugin 	|    📝   	|
