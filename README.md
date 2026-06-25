# harmonic-barcodes-3d-shape-classification

Research project at DePaul University implementing a matrix-based algorithm that
computes harmonic persistence barcodes for 3D shape classification.
September 2025 - Present.

## Research Problem

Standard topological data analysis captures when a shape feature (loop, void, connected
component) is born and when it dies - but throws away the actual geometric representative
that carried it. Harmonic chain barcodes preserve those representatives: they extract
the actual cycle generators that span each persistent homology class, carrying richer
geometric information than birth-death pairs alone.

The goal is to use these richer descriptors to classify 3D shapes that standard
persistence barcodes struggle to distinguish.

## Approach

The algorithm operates on boundary matrices derived from a simplicial complex built
over the 3D shape:

- Applies Gram-Schmidt orthogonalization to extract harmonic chain representatives
- Applies real-arithmetic corrections to handle numerical precision
- Extracts generator cycles from the orthogonalized basis
- Feeds the resulting feature vectors into SVM classifiers

## Shapes

Sphere, torus, cube, cylinder, cone, Mobius strip

## Stack

Python, GUDHI, NumPy, SciPy, scikit-learn

## Status

Implementation in progress.
