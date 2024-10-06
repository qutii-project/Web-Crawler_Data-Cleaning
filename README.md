# Overview
The notebook processes scientific document data from a JSON format, performs text cleansing, and extracts key information such as the title, DOI, and full-text content. The cleaned content is then saved in a PDF file.It parses JSON data, cleanses the text content, and generates a structured PDF report. This tool is useful for transforming raw data from research papers into readable, structured formats for further analysis.

# Key Functions
Text Cleansing:

Removes unwanted sections (e.g., references) and unwanted artifacts like figure/table/page references, non-ASCII characters, extra spaces, and erroneous punctuation.
Uses regular expressions to remove leading zeros from numbers and other text adjustments.
Encoding Fix:

Attempts to fix encoding issues in the text to handle potential formatting errors.
JSON Data Parsing:

Loads JSON data that includes text content and extracts key fields such as the title, DOI, and full-text URL.
Cleans the extracted content using the cleansing functions.
PDF Generation:

Uses the FPDF library to generate a PDF document with the extracted and cleaned content, including the title, DOI, and the full-text content.
Sample Workflow
Load a JSON file containing scientific data.
Extract the title, DOI, and full text.
Cleanse the text using the custom functions.
Output the cleaned text and extracted data to a structured PDF.

# Requirements
Python 3.x
Jupyter Notebook
Libraries:
json
re
fpdf (for generating PDF files)
You can install the required libraries using the following command:

bash
Copy code
pip install fpdf

# Features
Text Cleansing: Removes unwanted sections, figures, tables, and page references.
Data Extraction: Extracts title, DOI, and full-text content from JSON files.
PDF Report Generation: Generates a PDF with structured content, including the title, DOI, and full text.

# Usage
Load your scientific document in JSON format.
Run the notebook to extract key fields and cleanse the content.
A PDF file will be generated with the structured information.
