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

## Future Considerations
Due to the complex and technical nature of the content, it might be beneficial to explore other methods or services that can help refine the summaries.

1. **Refinement Using Advanced NLP Services:**
   - **OpenAI's GPT-3:** This service offers advanced natural language understanding capabilities. It is not free, but it allows for fine-tuning and prompting to enhance text clarity and coherence. By sending rough drafts to GPT-3 with specific instructions to refine the text, significant improvements can be achieved.
   - **Google's Cloud Natural Language:** Another paid service that provides tools for analyzing text structure and meaning. It can help refine summaries by identifying key points and rephrasing them for enhanced clarity.

2. **Free APIs and Tools for Summary Refinement:**
   - **SMMRY:** A free online tool that provides summarization services. Although it lacks a direct API for seamless integration into Python scripts without specific permissions, it can be manually used to assess summary quality.
   - **MeaningCloud Summarization API:** Offers a text summarization API that can assist in processing and refining summaries. It includes a free tier, which comes with limitations on the number of monthly requests.

3. **Implement Manual Post-Processing:**
   - **Regex and Text Processing:** Utilize custom Python scripts equipped with regular expressions to further refine summaries, addressing common textual errors and awkward phrasings.
   - **Custom Refinement Function:** Develop a function to identify and correct specific error patterns or complex jargon in the summaries, enhancing simplicity and clarity by providing additional context to the summarization model.


## Contributing
Contributions to this project are welcome! Please fork the repository and submit pull requests with your proposed changes.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
