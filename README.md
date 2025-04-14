I don't need to tell you how to unzip do i?
# Mega Millions Analysis Tool

This tool analyzes Mega Millions lottery data to identify patterns and generate predictions based on historical data.

## Features

- Extracts Mega Millions data from PDF files
- Analyzes number frequencies and patterns
- Generates predictions using multiple strategies
- Visualizes data through graphs and charts
- Tracks time between number occurrences
- Identifies hot and cold numbers

## Installation

1. Create a virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Place your Mega Millions PDF file in the `megamillions` directory
2. Run the extraction script:
```bash
python extract_pdf_data.py
```
3. Run the analysis:
```bash
python mega_millions_analyzer.py
```

## Analysis Results

Based on 215 draws analyzed, here are the key findings:

### Most Common Numbers

Regular Numbers:
- Number 3: 42 times (19.53%) from 2020-08-11 to 2024-12-24
- Number 1: 29 times (13.49%) from 2020-04-21 to 2025-03-25
- Numbers 7, 11, 15: 28 times each (13.02%)

Mega Ball Numbers:
- Numbers 19 and 22: 23 times each (10.70%)
- Number 20: 19 times (8.84%)
- Number 25: 17 times (7.91%)

### Least Common Numbers

Regular Numbers:
- Numbers 65, 67, 68: 1 time each (0.47%)
- Numbers 62, 66: 2 times each (0.93%)
- Numbers 63, 64, 57, 59, 61: 3-5 times each

Mega Ball Numbers:
- Numbers 2, 3, 4, 7: 1 time each (0.47%)
- Numbers 1, 5: 2 times each (0.93%)

### Prediction Strategies

1. **Frequency-based Strategy**
   - Based on most frequently occurring numbers
   - Current prediction: Regular numbers [3, 1, 7, 11, 15] with Mega Ball 19

2. **Hot Numbers Strategy**
   - Based on numbers that haven't appeared recently
   - Current prediction: Regular numbers [65, 67, 68, 62, 66] with Mega Ball 2

3. **Mixed Strategy**
   - Combines frequency and hot numbers approaches
   - Current prediction: Regular numbers [3, 1, 7, 65, 67] with Mega Ball 19

## Visualizations

The analysis generates two visualization files:
- `megamillions_frequency.png`: Shows the frequency distribution of numbers
- `megamillions_time_between.png`: Shows the time between number occurrences

## Notes

- The analysis is based on historical data and should not be used as the sole basis for lottery number selection
- Past performance does not guarantee future results
- The tool is for entertainment purposes only
- Please gamble responsibly

## Requirements

- Python 3.6+
- PyPDF2
- pandas
- matplotlib
- numpy 
