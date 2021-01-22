---
title: splinedist
layout: page
---

- *Contributor(s)*: Virginie Uhlmann, Soham Mandal (@sohmandal)
- *References*: [Github](https://github.com/uhlmanngroup/splinedist), [Preprint](https://www.biorxiv.org/content/10.1101/2020.10.27.357640v1)

## Purpose

> Describe the problem you are trying to solve by packaging your tool as a napari plugin in 1-2 sentences.
I should be able to read this alone and communicate the value to someone else.

### Why does this matter to biologists?

SplineDist provides vector representations of object outlines, which are more appropriate than pixel masks to do downstream shape analysis. Currently, SplineDist spits out mask segmentations because we do not have a good GUI allowing us to interactively edit its native output. Being able to interact with SplineDist output would allow editing segmentation mistakes, visualize the predicted cell outlines in their original form, and annotate training sets directly in SplineDist’s native data format.

### Why does this matter to you and your professional goals and responsibilities?

The Uhlmann group is focusing its efforts on method development. Since we are a small team, we usually only have the capacity to implement prototypes of our algorithms and cannot dedicate enough resources to designing GUIs and packaging the method in a fully user-friendly way. The interactive editing layer we would like to implement as part of napari’s SplineDist version would not only make the method more user-friendly, but also be immensely useful for several other shape analysis projects we have in which we rely on similar data types.

## Goals
> What would you like to accomplish during the Alfa Cohort collaboration?

1. Enable users to interactively manipulate (add, remove, edit) StarDist/SplineDist segmentation outlines.
2. Implement the interactive layer in a general enough manner (= such that it uses the Uhlmann group’s Python spline toolbox) to be reused in other future plug-ins relying on the same data type.

### Non-goals
> Are there any possible goals that are explicitly out of scope for the Alfa Cohort?

1. Edit StarDist/SplineDist core algorithmic routines in any way.
2. Create/implement a new library to handle spline models.

## Scope

### Key Features

During the Alfa Cohort
1. Interactive layer to interactively edit spline outlines (akin to the ImageCanvas and Roi extensions we have in Fiji) with companion toolbar - only drag/rotations/scaling
2. Save/load mechanisms in a simple file format (i.e. JSON)
3. Delete spline outline
4. Add spline outline - simple version: spawn default shape

Future considerations
1. Additional spline edit features - remove and add parameters
2. Add spline outline - advanced version: interpolate outline from bounding box


### Key Flows

> Show what the end-to-end experience will be for biologists.

A biologist will be able to
1. Run StarDist/SplineDist OR load existing StarDist/SplineDist results
2. Visualize segmentation results
3. Selecting any predicted object by clicking on it
4. Once selected, either
  1. Delete the entire outline
  2. Manually edit the outline in “spline mode” (TBD: dragging control points, adding control points, deleting control points?)
5. Create new spline models to delineate missed objects (TBD: spawn default circle shape or interpolate image content in a bounding box?)
6. Save results both as a mask and in spline format for further analysis or further editing


## Plan

### Milestones

> Status: To Do 📝, In Progress 🏗, In Review 🔎, Done ✅

| Target Date 	| Milestone 	| Description       	| Status 	|
|-------------	|-----------	|-------------------	|--------	|
|             	|           	|                   	|        	|
|             	|           	|                   	|        	|
| 2021-04-28  	| Demo day  	| Demo final plugin 	|    📝   	|
