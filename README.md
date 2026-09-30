# Business-Entity-Resolution
Business Entity Resolution using Python and similarity-based matching
# Business Entity Resolution using Python

## Project Overview

This project identifies whether different business records refer to the same real-world business.

## Objective

The system handles variations in business names and addresses and identifies possible matching business entities.

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Regex
- RapidFuzz
- KaggleHub

## Project Workflow

Dataset Loading
→ Data Cleaning
→ Text Normalization
→ Blocking
→ Candidate Generation
→ Similarity Calculation
→ Match Decision
→ Final CSV Output

## Dataset

The project uses three business data sources from the Amazon ML Challenge 2026 dataset.

- Source 1: 10,000 records used for validation
- Source 2: 5,034,616 records
- Source 3: 5,285,603 records

## Matching Method

Business names and addresses are compared using RapidFuzz similarity.

Final Score:

60% Name Similarity + 40% Address Similarity

## Validation Result

For 1,000 validation records:

- MATCH: 981
- POSSIBLE MATCH: 19
- NO MATCH: 0
- NO CANDIDATE: 0

## Output

The final matching results are saved in:

business_entity_resolution_results.csv
