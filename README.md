# NessusReporting
This Python script parses a Nessus vulnerability scan file (.nessus XML format) and generates a structured Word document (.docx) It categorizes vulnerabilities by severity (Critical, High, Medium, Low) and creates a report with tables detailing each vulnerability's name, criticality, synopsis, description, solution, and plugin output.

# Features
- Parses .nessus XML files using ElementTree.
- Categorizes vulnerabilities based on severity levels.
- Generates a formatted Word document using python-docx.
- Creates tables for each vulnerability with consistent styling (Arial, 10pt font).
- Saves the output report to a specified file path.

# Prerequisites

Python 3.x
Required Python packages:
  - xml.etree.ElementTree (standard library)
  - python-docx (install via pip install python-docx)

# Installation

1. Clone this repository:
git clone https://github.com/your-username/nessus-report-generator.git

2. Navigate to the project directory:
cd nessus-report-generator

3. Install the required package:
pip install python-docx

# Usage

1. Place your .nessus file in the desired directory.
2. Update the nessus_file_path variable in NessusScript.py with the path to your .nessus file.
3. Update the output_file_path variable in NessusScript.py with the desired path for the output Word document.
4. Run the script:

#> python NessusScript.py

The script will generate a Nessusreport.docx file in the specified output directory.

# Example

nessus_file_path = r"path\to\your\file.nessus"
output_file_path = r"path\to\output\Nessusreport.docx"

Ensure the .nessus file is accessible and correctly formatted.
