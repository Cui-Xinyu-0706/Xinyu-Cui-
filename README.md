# Satellite Annotation File Analysis - Advanced Data Handling

This project extends the previous analysis of satellite annotation files by applying data storage and serialization techniques. Using Python libraries such as JSON and Pickle, this project organizes annotations by date and enables efficient data storage and retrieval. The project also includes filtering and sorting of annotations based on specific date ranges.

## Table of Contents

- [Overview](#overview)
- [Objectives](#objectives)
- [Requirements](#requirements)
- [Usage](#usage)
- [Output](#output)
- [License](#license)

## Overview

This project builds on the satellite annotation analysis by:
1. Counting annotations per month and year.
2. Structuring and saving data in JSON and Pickle formats.
3. Organizing annotation metadata using dictionaries and sorting by specific date ranges.

## Objectives

The project achieves the following:

1. **Annotations by Month and Year**: Count the number of annotations for each month and year and identify the month with the most annotations.
2. **Monthly Annotations Dictionary**:
   - Create a dictionary where each **key** represents a month, and the **value** is a list of all annotation names for that month.
   - Save the dictionary in both **JSON** and **Pickle** formats to verify its integrity.
   - Extend the dictionary structure to store each annotation as a dictionary with `name` and `date` (using a datetime object).
3. **Filter and Sort Annotations by Date**: Print all annotations occurring in the second half of 2024, sorted from the oldest to the newest.

## Requirements

- **Python 3.x**
- Libraries:
  - **json**: For JSON serialization and deserialization.
  - **pickle**: For binary serialization.
  - **datetime**: For date handling and filtering.
  - **os**: For file handling.

## Usage

1. **Clone the Repository**:
   ```bash
   git clone <repository_url>
   cd <repository_folder>

