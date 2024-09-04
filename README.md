# Web Crawler and Data Cleansing Pipeline
# Overview

This project is a Python-based pipeline designed for web scraping and subsequent data cleansing. The pipeline reads data from an Excel file, consolidates it into a single textual format, and applies a series of cleaning operations to remove unwanted sections, characters, and inconsistencies from the text.
Features

    Data Loading: Load data from an Excel file using Pandas.
    Text Consolidation: Merge multiple columns of data into a single "text" column for processing.
    Text Cleansing:
        Removal of unwanted sections such as "abstract", "methods", and "references".
        Elimination of non-ASCII characters and excessive whitespace.
        Correction of formatting issues (e.g., leading zeros in numbers).

# Requirements

To run the code, make sure you have the following Python libraries installed:

    pandas
    nltk
    openpyxl
    spacy
    numpy

You can install these by running:

bash

pip install -r requirements.txt

# How to Use

    Input Data: Place your Excel file (e.g., filename.xlsx) in the root directory.
    Run the Notebook:
        Load the Excel file into a Pandas DataFrame.
        Consolidate the data into a single text column.
        Apply the cleansing functions provided in the notebook to process the text.
    Functions:
        cleanse_text(text): Cleans the text by removing unwanted sections and fixing formatting issues.
        remove_leading_zeros(text): Removes unnecessary leading zeros from numbers.
# Output

The output will be a DataFrame with a csv cleansed version of the text that can be exported or used for further analysis.
