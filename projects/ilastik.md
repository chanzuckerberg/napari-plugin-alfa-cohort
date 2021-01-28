---
title: Ilastik
layout: page
---

- *Contributor(s)*: Emil Melnikov (@emilmelnikov), Dominik Kutra (@k-dominik), Anna Kreshuk (@akreshuk)
- *References*: [Project Site](https://www.ilastik.org/), [Github](https://github.com/ilastik), [Publication](https://www.nature.com/articles/s41592-019-0582-9)

## Purpose

> Describe the problem you are trying to solve by packaging your tool as a napari plugin in 1-2 sentences.
I should be able to read this alone and communicate the value to someone else.

### Why does this matter to biologists?

The ilastik plugin allows Biologists to perform semantic segmentation on their images.
Having this available in a common framework with other tools enables complex analysis pipelines and interactive exploration.

### Why does this matter to you and your professional goals and responsibilities?

Since napari is expected to be a widely adopted Python-based image viewer, we would like to be a part of a broader ecosystem.
Moreover, using napari could lower the maintenance efforts of maintaining an image viewer component for the ilastik development team.

## Goals

> What would you like to accomplish during the Alfa Cohort collaboration?

1. Offer "bread and butter" classic Ilastik pixel-based classifier application as a napari plugin
2. Evaluate napari's opportunity to support other tools that the Ilastik group is developing

### Non-goals

> Are there any possible goals that are explicitly out of scope for the Alfa Cohort?

1. Do not want to replace support for “classic” Ilastik

## Scope

### Key Flows

> Show what the end-to-end experience will be for biologists.

A biologist will be able to
1. Load data
2. Select filters to compute and use as features
3. Interactively label
4. Evaluate results
5. Predict everything
6. Export
7. Save project to be used in batch mode

## Plan

### Milestones

> Status: To Do 📝, In Progress 🏗, In Review 🔎, Done ✅

| Target Date | Milestone      | Description                                                                                                                                                          | Status |
|-------------|----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|
| 2021-02-24  | Fixed Pipeline | The plugin works with the predefined set of features. There is no interactive labelling yet: as a temporary solution, labels should be loaded from an external file. | 📝      |
| 2021-03-17  | Interaction    | Dataset can be labelled interactively.                                                                                                                               | 📝      |
| 2021-04-07  | Filters        | Filters are selectable.                                                                                                                                              | 📝      |
| 2021-04-28  | Batch and Demo | Images can be processed in a batch mode. Present the final plugin.                                                                                                   | 📝      |
