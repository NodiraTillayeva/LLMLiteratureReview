# Literature Review Assistant

A Jupyter Notebook-based tool to streamline the literature review process. It helps you analyze and rank academic papers from Web of Science and PubMed based on their relevance to your research topic using OpenAI's API.

---

## Features

- **Automated Relevance Scoring**: Uses OpenAI to assess relevance of papers based on title, abstract, and metadata.
- **Web of Science & PubMed Integration**: 
  - Web of Science: Papers saved manually from the website.
  - PubMed: Papers retrieved using PubMed API.
- **Customizable Evaluation**: Define or tweak relevance criteria.
- **Ranked Results**: Produces a sorted list of papers with relevance scores, keywords, and links.

---

## Example Input Table

| Title                                               | DOI                        | Abstract Snippet                     |
|-----------------------------------------------------|-----------------------------|--------------------------------------|
| Human movement and disease spread                   | 10.1016/j.jtbi.2022.111367 | Analyzes the role of mobility in...  |
| Infectious diseases in urban networks               | 10.1073/pnas.2007488118    | Compares disease models in cities... |

---

## Example Output Table

| Title                          | Relevance | Disease        | Region   | Citations |
|-------------------------------|-----------|----------------|----------|-----------|
| Human migration & infection   | 8.0       | General        | Global   | 43        |
| Modeling Dengue Persistence   | 9.0       | Dengue         | Tropics  | 14        |

---

## Getting Started

### Prerequisites

- Python 3.7+
- Libraries: `pandas`, `numpy`, `openai`

Install with:
```bash
pip install -r requirements.txt
```

### API Key Setup
Get your key from [OpenAI](https://platform.openai.com/). Then:
```bash
export OPENAI_API_KEY=your_api_key_here
```
Or set it inside the notebook directly.

### Running the Tool
```bash
git clone https://github.com/yourusername/literature-review-assistant.git
cd literature-review-assistant
jupyter notebook literature_review.ipynb
```

---

## Workflow

1. Export data from Web of Science as CSV (manual download).
2. Retrieve PubMed papers using the built-in API method.
3. Load the files into the notebook.
4. Set your research topic.
5. Run cells to analyze and score the papers.
6. View sorted output to prioritize your reading.

---

## Customization Options

- **Relevance Prompts**: Change how papers are scored by modifying GPT prompts.
- **Weight Adjustments**: Tune how importance is given to keywords, titles, abstracts.
- **Support for More Sources**: Add parsing for Scopus, IEEE, etc.

---

## Output Includes

- Titles
- Abstracts
- Authors
- Relevance Scores
- Citation Counts
- Disease/Region Tags (if applicable)
- Direct links (DOIs)

---

## Notes

- Choose between GPT-3.5 or GPT-4 depending on precision vs speed/price.
- Monitor API usage; large datasets may consume significant tokens.

---

## License
MIT License - see [LICENSE](LICENSE)

---

Contributions welcome! Feel free to open issues or pull requests.

Happy researching! 🚀
