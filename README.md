# Whole-Tree Modeling from LiDAR Point Clouds Using Heat-Diffusion-Guided Skeletonization and Spherical-Harmonic Crown Representation

This repository provides the code implementation for:

**Whole-Tree Modeling from LiDAR Point Clouds Using Heat-Diffusion-Guided Skeletonization and Spherical-Harmonic Crown Representation**

The framework reconstructs whole-tree structure from LiDAR point clouds by integrating **heat-diffusion-guided branch skeletonization** and **spherical-harmonic-based crown representation**. It supports unified modeling of woody architecture and crown morphology, including branch skeleton extraction, QSM generation, and crown morphology encoding.

---

## Overview

The proposed method contains two main components:

1. **Heat-diffusion-guided skeletonization**  
   A bottom-up heat-diffusion field is constructed on woody point clouds to estimate growth-trend vectors, which guide branch trajectory tracing and topology refinement.

2. **Spherical-harmonic crown representation**  
   Foliage points are mapped onto a spherical radial representation, and crown morphology is encoded using spherical harmonics to obtain a compact and continuous crown model.

The overall goal is to provide a unified whole-tree representation that links internal woody architecture with external crown morphology.

---

## Graphical User Interface

The repository includes a graphical user interface for loading LiDAR point clouds, performing whole-tree modeling, and visualizing reconstruction results.

![Operation Interface](pictures/figure1.png)

---

## Method Principle

The principle of the proposed framework is illustrated below. The workflow includes heat-diffusion-based growth-trend estimation, streamline-guided skeleton extraction, QSM reconstruction, and spherical-harmonic crown modeling.

![Method Principle](pictures/figure2.png)

---

## Repository Structure

```text
.
├── app.py
├── pipeline/
├── io_utils/
├── ui/
├── pictures/
│   ├── figure1.png
│   └── figure2.png
├── outputs/
├── cache/
└── README.md
