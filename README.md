# Literature Review Assistant

A Jupyter Notebook tool for analyzing academic papers from Web of Science and PubMed using OpenAI's API to score relevance.

## Features
- **Automated Relevance Scoring**: Evaluates abstracts/keywords against research topics
- **Dual-Source Support**: Processes Web of Science CSV exports and PubMed API data
- **Customizable Criteria**: Adjust scoring weights for disease focus, methodology, etc.
- **Unified Output**: Generates ranked lists with scores and key metadata

## Input Formats

### Web of Science (CSV)
| Authors | Article Title | Journal | Year | DOI |
|---------|---------------|---------|------|-----|
| Smith A | Disease modeling... | Nature | 2023 | 10.123/abc |

### PubMed (API)
| PMID | Title | Journal | Year | Abstract Excerpt |
|------|-------|---------|------|------------------|
| 12345 | Climate impacts... | Science | 2022 | "Temperature changes..." |

## Sample Output
| Title | DOI | Source | Score | Key Findings |
|-------|-----|--------|-------|--------------|
| Human mobility... | 10.123/xyz | WoS | 9.1 | "Commuting explains 70%..." |

## Setup
```bash
pip install pandas numpy openai biopython
export OPENAI_API_KEY="sk-your-key-here"
