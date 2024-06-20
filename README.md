## Readme

# Legal Question-Answering System

## Overview

The Legal Question-Answering System leverages Google Generative AI to answer legal questions intelligently based on a corpus of legal documents. The system currently supports multiple law domains, including:

- Criminal Law
- Civil Law (implementation pending)
- Indian Divorce Act (implementation pending)
- Motor Vehicle Act (implementation pending)

Users can interact with the system by selecting their domain of interest and posing their legal questions. The system processes the query, retrieves the most relevant legal passage, and generates an informative and concise answer.

## Features

- **Multi-Domain Support**: Users can query different domains of law.
- **Intelligent Answer Generation**: Uses Google Generative AI for generating comprehensive and context-aware answers.
- **Context Retrieval**: Embeds and retrieves the most relevant passage from the dataset based on the user's query.
- **Friendly and Conversational Tone**: The system responds in a manner that is easy to understand for non-technical users.

## Setup

### Prerequisites

- Python 3.x
- Pandas
- NumPy
- Google Generative AI

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/legal-qna-system.git
   cd legal-qna-system
   ```

2. Install the required packages:

   ```bash
   pip install pandas numpy google-generativeai langchain-google-genai
   ```

3. Set up your Google API key:

   ```python
   import os
   os.environ['GOOGLE_API_KEY'] = "YOUR_GOOGLE_API_KEY"
   ```

### Data Preparation

1. Place the `criminal_embed.csv` file in the root directory.
2. (Optional) Prepare other domain datasets (`civil_embed.csv`, `ida_embed.csv`, `mva_embed.csv`).

### Running the System

1. Execute the main script:

   ```bash
   python main.py
   ```

2. Follow the prompts to select your law domain and enter your legal question.

## Example Usage

```bash
Choose your law domain to ask questions (Type number):
1. Criminal
2. Civil
3. Indian Divorce Act
4. Motor Vehicle Act
 Your choice: 1

Your Legal Questions?

What is the punishment for theft?
```

## Future Scope

- **Extend to More Law Domains**: Add support for additional law domains.
- **Enhanced Query Processing**: Improve query understanding and processing capabilities.
- **User Interface**: Develop a user-friendly web or mobile interface for easier interaction.
- **Multilingual Support**: Enable the system to handle queries in multiple languages.
- **Advanced Analytics**: Incorporate analytics to provide insights into frequently asked questions and legal trends.

## Contributing

We welcome contributions to improve the system. Please follow the standard fork-pull request workflow and ensure that your code adheres to the project's coding standards.

## License

This project is licensed under the MIT License. See the [Apache License 2.0] file for details.

## Contact

For any questions or suggestions, feel free to open an issue or contact us at [yashsinghmain2002@gmail.com].

