# From CSV to Word – Automated Document Generation with Python

## Project Overview
A Python script that automatically generates a Word document (.docx) from 
a CSV file. For each row of the CSV, a formatted table is created in the 
document, with field names in the left column and the corresponding values 
in the right column. Each table is separated by a page break, resulting in 
a clean, one-record-per-page document.

This script was developed for a museum, to automate the creation of 
catalogue sheets for a collection of artefacts.

## How It Works
1. The CSV file is read with Pandas
2. Column names are normalised for consistency
3. Duplicate records are removed
4. Unnecessary columns are dropped
5. Null values are replaced with empty strings
6. A Word document is generated with one formatted table per row
7. The document is saved and downloaded

## Features
- Automatic column renaming for data normalisation
- Duplicate removal based on inventory number
- Null value handling
- Customisable Word document formatting (font, margins, table style)
- One catalogue sheet per page, ready to print or share

## Technologies Used
- Python
- Pandas
- NumPy
- python-docx
- Google Colab
- Google Drive

## Notes
The script was developed and run on Google Colab, with the input CSV file 
stored on Google Drive. File paths can be adapted to run locally by 
replacing the Google Drive mount with a local path — for example, 
using Visual Studio Code or any other local Python environment.
