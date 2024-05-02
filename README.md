# ML Document Classifier using Huggingface

## Overview
This Document Processing Toolkit provides a comprehensive solution for scanning files in a specified directory, extracting text, generating tags based on content, and summarizing the text using Hugging Face's transformers. It supports multiple file formats including PDF, DOCX, TXT, and CSV. This toolkit is ideal for managing large volumes of documents, providing quick insights, and organizing content efficiently.

## Features
- **Text Extraction**: Supports PDF, DOCX, TXT, and CSV files.
- **Text Cleaning**: Includes special handling for character and punctuation spacing and removing extra whitespace.
- **Semantic Tagging**: Uses topic modeling to generate relevant tags from the content.
- **Summarization**: Utilizes Hugging Face's BART large model to create concise summaries.
- **Spell Checking**: Corrects spelling mistakes in the summaries using a simple spell checker.

## Requirements
To run this toolkit, you will need Python 3.x and the following packages:
- `pdfplumber`
- `python-docx`
- `pandas`
- `re`
- `transformers`
- `spellchecker`
- `nltk`
- `gensim`

You can install these packages via pip:
pip install pdfplumber python-docx pandas re transformers pyspellchecker nltk gensim


## Usage
To use this toolkit, follow these steps:

1. Clone this repository to your local machine.
2. Install all required dependencies.
3. Place your documents in the `testdocuments` directory or specify your directory.

Run the script :)

## Example Output
The toolkit will process each file in the directory and output the following for each file:
- **File Name**: The name of the processed file.
- **Tags**: Semantic tags generated from the content.
- **Summary**: A concise summary of the content.

## Contributing
Contributions to this project are welcome! Please fork the repository and submit pull requests with your proposed changes.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
