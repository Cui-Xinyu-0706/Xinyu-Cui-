# Satellite Annotation File Analysis

This project processes a set of satellite annotation files within a ZIP archive, following a specific filename convention. The program extracts information from these files, organizes them by date and satellite, and provides summary statistics.

## Table of Contents

- [Overview](#overview)
- [Filename Convention](#filename-convention)
- [Objectives](#objectives)
- [Requirements](#requirements)
- [Usage](#usage)
- [Output](#output)
- [License](#license)

## Overview

This project performs a detailed analysis on a collection of satellite annotation files with a defined naming pattern. It calculates summary statistics, organizes the files by month, and presents key insights based on the provided annotations.

## Filename Convention

Each annotation file follows the naming convention:

`{DATE}_{TIME}_SN{SATELLITE_NUMBER}_QUICKVIEW_VISUAL_{VERSION}_{UNIQUE_REGION}.txt`

Where each component is defined as follows:
- **DATE**: In `YYYYMMDD` format, e.g., `20241201` or `20230321`
- **TIME**: In `HHMMSS` format, e.g., `2134307`
- **SATELLITE_NUMBER**: An integer representing the satellite number
- **VERSION**: Pipeline version, e.g., `0_1_2` or `1_3_1`
- **UNIQUE_REGION**: String defining a specific region, e.g., `SATL-2KM-10N_552_4164`

## Objectives

The program achieves the following objectives:

1. **Count Files**: Determine the total number of files in the annotations folder.
2. **Name Convention Check**: Count files that adhere to the specified naming convention.
3. **Monthly and Yearly Annotations**: Count annotations per month and year, and identify the month with the highest number of annotations.
4. **Organize by Month**: Create a new folder structure where each subfolder corresponds to a month.
5. **Sort Annotations by Date**: Print all annotations from the most recent to the oldest.
6. **Satellite Analysis**:
   - Count unique satellites.
   - Calculate annotations per satellite.
   - Identify the satellite used in the most recent annotation file.
7. **Unique Regions**: Count the number of unique regions.

## Requirements

- **Python 3.x**
- **numpy** for sorting operations
- **os** and **zipfile** libraries for file handling

## Usage

1. **Clone the Repository** and extract the ZIP file:
   ```bash
   git clone <repository_url>
   cd <repository_folder>

