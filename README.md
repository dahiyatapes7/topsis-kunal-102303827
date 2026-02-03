TOPSIS 

This project implements the Technique for Order Preference by Similarity to Ideal Solution (TOPSIS) using Python.

The program works as a command line tool and ranks alternatives based on multiple criteria, weights and impacts.

---

Requirements

- Python 3.x
- pandas
- numpy

---

Folder Structure

Topsis-Kunal-102303827/
│
├── setup.py
├── README.md
├── LICENSE
│
└── topsis/
    ├── __init__.py
    └── topsis.py

---

Command Line Usage

python topsis.py <InputDataFile> <Weights> <Impacts> <OutputFile>

Example:

python topsis.py data.csv "1,1,1,2" "+,+,-,+" result.csv

---

Input File Format

- Input file must be a CSV file
- Minimum three columns are required
- First column should contain alternatives (non-numeric)
- Remaining columns must contain numeric values only

---

Conditions Checked by Program

- Correct number of command line arguments
- File not found handling
- Minimum column requirement
- Numeric validation of criteria columns
- Number of weights equals number of impacts and criteria
- Impacts must be either + or -

---

Output

The output file will be a CSV file containing:
- Topsis Score
- Rank

Higher Topsis score indicates a better alternative.

---

Author

Name: Kunal Dahiya  
Roll Number: 102303827  
