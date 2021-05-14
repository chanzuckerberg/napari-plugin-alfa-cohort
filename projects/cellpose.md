---
title: cellpose
layout: page
---

- *Contributor(s)*: Carsen Stringer (@carsen-stringer)
- *References*: [Project Site](http://www.cellpose.org/), [Github](https://github.com/MouseLand/cellpose), [Documentation](https://cellpose.readthedocs.io/en/latest/outputs.html), [Publication](https://www.biorxiv.org/content/10.1101/2020.02.02.931238v2)

## Purpose

> Describe the problem you are trying to solve by packaging your tool as a napari plugin in 1-2 sentences.
I should be able to read this alone and communicate the value to someone else.

### Why does this matter to biologists?
Segmentation of cells is an important step in a variety of biological processing workflows. A single segmentation algorithm may not work for all data types and therefore an easy way for a biologist to combine pre-processing steps and try a variety of deep learning algorithms is essential. Napari is an easy-to-use single package for the biologist to filter and process their images.

### Why does this matter to you and your professional goals and responsibilities?
Providing biologists’ accessibility to complex tools is one of my major professional responsibilities as an algorithm developer.

## Goals
> What would you like to accomplish during the Alfa Cohort collaboration?

1. Run 2D & 3D pre-trained cellpose in napari
2. Save 2D annotations in a way that they can be loaded through cellpose CLI for training
3. “How did I run this?” Support serialization of parameters for provenance tracking.

### Non-goals
> Are there any possible goals that are explicitly out of scope for the Alfa Cohort?

1. Training cellpose model in the napari GUI
2. Batch mode

## Scope

### Key Flows

> Show what the end-to-end experience will be for biologists.

A biologist will be able to

1. Load their data (2D or 3D)
1. Choose a model (pre-trained from cellpose team OR specify their own)
1. Choose what channels to run on & other parameters
1. Run cellpose on the current data
1. View the results
1. Modify / curate data in a flexible way (handles on cells & reshape if they don’t like the boundaries)
1. Save results for further analysis

A savvy biologist will be able to
1. Load training data in 2D
1. Annotate cells
1. Export/save the annotations
1. Run cellpose CLI on annotated data
1. View results
1. Apply trained model as above


## Plan

### Milestones

> Status: To Do 📝, In Progress 🏗, In Review 🔎, Done ✅

| Target Date 	| Milestone 	| Description       	| Status 	|
|-------------	|-----------	|-------------------	|--------	|
|             	|           	|                   	|        	|
|             	|           	|                   	|        	|
| 2020-04-28  	| Demo day  	| Demo final plugin 	|    📝   	|

## Outcomes

- [cellpose-napari](https://github.com/mouseland/cellpose-napari)
- [Twitter announcement](https://twitter.com/computingnature/status/1389037192375410688)
