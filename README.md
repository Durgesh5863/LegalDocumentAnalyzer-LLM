# Legal Document Analyzer

A powerful tool leveraging Large Language Models (LLM) to analyze, summarize, and extract insights from legal documents.

## Overview

The Legal Document Analyzer is designed to help legal professionals, researchers, and organizations efficiently process and understand legal documents. By utilizing advanced natural language processing and machine learning techniques, this tool can:

- Extract key information from legal documents
- Generate concise summaries of lengthy legal texts
- Identify important clauses and provisions
- Compare multiple documents for similarities and differences
- Provide insights and analytics on legal content

## Features

- **Document Processing**: Upload and process PDF legal documents
- **Intelligent Analysis**: Leverage LLM capabilities to understand legal terminology and context
- **Summary Generation**: Create concise summaries of complex legal documents
- **Key Information Extraction**: Automatically identify parties, dates, amounts, and other critical elements
- **Clause Identification**: Extract specific clauses like payment terms, confidentiality, termination, and governing law
- **Risk Analysis**: Identify potential risk factors in legal documents
- **Named Entity Recognition**: Extract and categorize named entities in legal text

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Required Python packages (see requirements.txt)
- Access to pre-trained language models

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/Durgesh5863/LegalDocumentAnalyzer.git
   cd LegalDocumentAnalyzer
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Download the required spaCy model:
   ```
   python -m spacy download en_core_web_sm
   ```

## Usage

### Jupyter Notebook

The main functionality is provided through the `document_analyzer.ipynb` Jupyter notebook. Open the notebook to analyze legal documents:

```
jupyter notebook document_analyzer.ipynb
```

### Core Functions

The analyzer provides several key functions:

1. **Text Extraction**: Extract text from PDF documents
   ```python
   pdf_text = extract_text_from_pdf('path/to/your/document.pdf')
   ```

2. **Document Summarization**: Generate concise summaries of legal documents
   ```python
   summary = generate_summary(pdf_text)
   ```

3. **Entity Extraction**: Identify and categorize named entities in the document
   ```python
   entities = extract_entities(pdf_text)
   ```

4. **Clause Extraction**: Extract specific types of clauses from the document
   ```python
   clauses = extract_clauses(pdf_text)
   ```

5. **Risk Analysis**: Identify potential risk factors in the document
   ```python
   risks = analyze_risks(clauses)
   ```

## Example Output

The analyzer provides structured output including:

- Document summary
- Named entities (parties, dates, amounts, etc.)
- Extracted clauses (payment terms, confidentiality, termination, governing law)
- Risk analysis highlighting potential issues in the document

## Models Used

- **Legal-BERT**: Fine-tuned BERT model for legal text understanding
- **BART-CNN**: For document summarization
- **spaCy**: For named entity recognition and text processing

## Limitations

- Currently supports PDF documents only
- Performance depends on the quality and structure of the input document
- May not recognize highly specialized legal terminology in certain domains

## Future Enhancements

- Support for additional document formats (DOCX, TXT)
- Improved clause extraction with more categories
- Custom training for specific legal domains
- Web interface for easier document processing
- Batch processing for multiple documents

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- HuggingFace Transformers library
- PyMuPDF for PDF processing
- spaCy for NLP tasks