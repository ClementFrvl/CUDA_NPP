# CUDA NPP Filtering Lab

## Project Overview

This project serves as a sandbox for exploring the filtering and image processing capabilities provided by the CUDA NPP (NVIDIA Performance Primitives) Library. It currently implements several well-known filters, including:

- **Canny Edge Detection Filter** (`canny`)
- **Sobel Edge Detection Filter** (`sobel`)
- **Gaussian Smoothing Filter** (`gauss`)
- **Sharpening Filter** (`sharpen`)

The program allows users to apply one of these filters to an image (in BMP or PGM format), specifying both the filter and the output file or directory for the processed image. 

At present, the application processes only one image at a time due to an issue with NPP kernel execution, which fails when attempting to rerun the same kernel multiple times.

The project is designed to be executed within a Coursera Lab environment, where the required CUDA setup is pre-configured. For now, additional environment configuration falls outside the scope of this project.

## Project Structure

```
bin/
```
Contains all the binary/executable files generated during the build process. Executables will follow the `.exe` extension or an appropriate extension based on the programming language.

```
data/
```
Houses sample input data files (images) in any supported format. For large datasets, this directory may be left empty, with scripts or instructions provided to download the necessary files.

```
lib/
```
Includes any external libraries that are not installed through the system's package manager, ensuring that all dependencies are easily accessible for linking or inclusion.

```
src/
```
Contains the project's source code, structured hierarchically as needed.

```
README.md
```
This file provides an overview of the project, helping potential users or contributors quickly understand its purpose and scope.

```
INSTALL
```
Contains detailed instructions on how to install and configure the project. It should cover installation steps for multiple operating systems if applicable, to maximize accessibility.

```
Makefile`
```
Provides scripts for building the project automatically, depending on the system's preferred build tools.

```
run.sh
```
(Optional) A script for running the compiled executable, with or without additional command-line arguments.
