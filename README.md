# Novel Topological Descriptors for Topological Data Analysis
Research project at DePaul University developing harmonic chain barcodes as
novel topological descriptors for shape and point cloud analysis.
September 2025 - Present.

## Research Problem

Standard persistence barcodes capture when topological features are born and die
but discard the actual geometric representatives that carried them. Harmonic chain
barcodes preserve those representatives - extracting the cycle generators that span
each persistent homology class and carrying richer geometric information than
birth-death pairs alone.

This project investigates how these harmonic chain representatives behave, persist,
and remain stable across different inputs.

## Algorithm

- Builds boundary matrices from a simplicial complex over the input data
- Applies Gram-Schmidt orthogonalization to extract harmonic chain representatives
- Applies real-arithmetic corrections for numerical precision
- Extracts generator cycles from the orthogonalized basis
- Converts barcodes to persistence images
- Feeds persistence image features into SVM classifiers

## Experiments

**Shape Experiments**
Testing the harmonic barcode pipeline on standard geometric shapes to evaluate
how well the extracted features distinguish different topologies.

**Random Point Cloud Experiments**
Generating random point clouds and testing whether harmonic barcode features
can identify structural patterns across many randomly generated inputs.

## Stack

Python, GUDHI, NumPy, SciPy, scikit-learn

## Status

Implementation in progress.
