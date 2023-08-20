# Symmetric Non-negative Matrix Factorization (SymNMF) for Clustering

## Overview
This project implements a clustering algorithm based on symmetric Non-negative Matrix Factorization (SymNMF). The algorithm is applied to several datasets and is compared with the K-means clustering method. The main goal is to form clusters based on the provided data points.

## Features
- Implementation in both C and Python.
- Python-C interface for efficient computation.
- Analysis tool to compare SymNMF with Kmeans clustering.

## Dependencies
- Python 3.x
- GCC Compiler
- Python's numpy module

## How to Run
### Compilation:
To compile the C module:
$make
To build the Python extension:
$python3 setup.py build_ext --inplace
### Execution:
For the Python program:
$python3 symnmf.py <k> <goal> <input_file.txt>
For the C program:
$./symnmf <goal> <input_file.txt>
For analysis comparing SymNMF with Kmeans:
$python3 analysis.py <k> <input_file.txt>

## File Structure
- symnmf.py: Main Python interface.
- symnmf.c: C implementation of the SymNMF algorithm.
- symnmfmodule.c: Python C API wrapper for interfacing with the C module.
- symnmf.h: C header file.
- analysis.py: Analysis tool to compare SymNMF with Kmeans.
- setup.py: Python build script.
- Makefile: Make script for building the C interface.

## Acknowledgements
The project is based on the paper:

> Da Kuang, Chris Ding, and Haesun Park. "Symmetric nonnegative matrix factorization for graph clustering." In Proceedings of the 2012 SIAM International Conference on Data Mining (SDM).
