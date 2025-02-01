# Genomic Variant Annotation and EDA

This repository contains code for performing Exploratory Data Analysis (EDA) on genomic variant data and functional annotation using PyRanges.

## Overview

The project focuses on the following tasks:
- **Exploratory Data Analysis (EDA)**: The data is analyzed to uncover patterns, relationships, and useful insights for variant information.
- **Functional Annotation**: Genomic variants are annotated with relevant information to facilitate downstream analysis, such as assessing their potential impact.

## Dependencies

The following libraries are required to run the code:

- pandas
- pyranges
- matplotlib
- seaborn
- scipy
- numpy

To install them you can download the requirements file and run pip install -r requirements.txt

## Code Description

### 1. **Exploratory Data Analysis (EDA)**

The **EDA** code aims to load genomic variant data, visualize and analyze the dataset to detect patterns or anomalies that could provide useful insights for downstream processing or research. In this case, the variant data consists of chromosomes, positions, reference sequences, and alternate sequences for genetic variants.

Key components of the EDA:
- **Chromosome**: The chromosome on which the variant is located.
- **Start** and **End**: The starting and ending positions of the variant.
- **Ref**: The reference sequence at the variant position.
- **Alt**: The alternate sequence for the variant.

The goal of this part is to display the variant data, calculate basic statistics, and explore the data for any significant trends or distributions.

### 2. **Functional Annotation**

This part of the code takes genomic variant data (e.g., from df7) and performs **functional annotation** by joining or intersecting it with existing annotations to enrich the variant data. The functional annotation process can help identify **potential functional consequences of variants**, such as whether they affect coding regions or regulatory elements.

- **Variant Data**: The first dataset represents genetic variants including chromosome, position, reference, and alternate alleles.
- **Annotation Data**: The second dataset provides annotations for the variants, such as chromosome positions and reference/alternate information for comparison.

The key steps are:

**Create PyRanges objects**: PyRanges is used to store and manipulate genomic range data.
**Join the variant and annotation datasets**: This operation finds overlapping regions between variants and annotations, annotating the variants with additional information.

##Conclusion
This repository helps perform key tasks in genomic analysis, such as exploratory data analysis and functional annotation, using the PyRanges library. These tasks are critical in understanding the genetic variants' potential functional impact and their relevance in different biological contexts.





