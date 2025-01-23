
# Literature Review Assistant

This repository contains a Jupyter Notebook designed to streamline the literature review process by analyzing papers from the Web of Science. The tool uses the OpenAI API to evaluate and score the relevance of each paper for a specific discussion or research paper, helping researchers focus on the most relevant literature.

## Features

- **Automated Relevance Scoring**: Uses the OpenAI API to analyze keywords, abstracts, and metadata for relevance to your research topic.
- **Web of Science Integration**: Processes exported data from the Web of Science for analysis.
- **Customizable Scoring Criteria**: Adjust the relevance evaluation to align with specific research goals.
- **Detailed Outputs**: Produces a ranked list of papers based on their relevance to your topic.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Python 3.7 or higher
- Required libraries:
  - `pandas`
  - `numpy`
  - `openai`

Install the dependencies using:

```bash
pip install -r requirements.txt
```

### OpenAI API Key

To use the OpenAI API, you need an API key. Sign up at [OpenAI](https://platform.openai.com/) to obtain your API key.

Set up your API key as an environment variable:

```bash
export OPENAI_API_KEY=your_api_key_here
```

Or configure it directly in the notebook where indicated.

### Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/literature-review-assistant.git
   cd literature-review-assistant
   ```

2. Open the Jupyter Notebook:

   ```bash
   jupyter notebook literature_review.ipynb
   ```

3. Upload your Web of Science export file or dataset for analysis.

4. Define your research topic and adjust the scoring criteria.

5. Run the notebook cells to process the data, analyze the papers using the OpenAI API, and generate relevance scores.

6. Review the ranked list of papers and use it to guide your literature review.

## Example Workflow

1. Export search results from the Web of Science as a CSV file.
2. Load the CSV file into the Jupyter Notebook.
3. Set your research topic and customize scoring parameters.
4. Analyze the papers using the OpenAI API.
5. Review the output, which includes ranked papers and their relevance scores.

## Customization

- **Scoring Algorithm**: Modify the criteria for relevance scoring by adjusting the API prompts or weighting factors in the notebook.
- **Additional Data Sources**: Extend the notebook to process data from other bibliographic platforms or APIs.

## Output

The notebook generates a structured output that includes:

- Paper titles
- Abstracts
- Authors
- Relevance scores
- Links to original publications (if available)

## Notes on the OpenAI API

- Ensure you have sufficient API usage credits on your OpenAI account.
- You can adjust the API model (e.g., `gpt-3.5-turbo` or `gpt-4`) in the notebook.

## Contributions

Contributions are welcome! If you encounter a bug or have a feature request, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Happy researching! 🚀
