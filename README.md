# Gemini Embedding Model Test

This project demonstrates how to use the Google Gemini Embedding Model to create text embeddings.

## Description

This code uses the `google.generativeai` library to perform the following tasks:
- Load an API key from a `.env` file.
- Configure the Gemini API.
- Select an embedding model.
- Embed a sample text.
- Print the resulting embedding and its dimensions.
- List available embedding models and their properties.

## Requirements

- Python 3
- `google-generativeai`
- `python-dotenv`

## Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/kshLithium/gemini-embedding.git
    cd gemini-embedding
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: A `requirements.txt` file is not present. You can create one with the following content:)*
    ```
    google-generativeai
    python-dotenv
    ```

3.  **Create a `.env` file:**
    Create a file named `.env` in the root directory and add your API key:
    ```
    GEMENI_API_KEY="YOUR_API_KEY_HERE"
    ```

## Usage

Open and run the cells in the `test.ipynb` Jupyter Notebook to see the embedding process in action.

## Code Explanation

- **Import libraries:** Imports `google.generativeai` for the AI model and `dotenv` to manage environment variables.
- **Load API Key:** Loads the `GEMENI_API_KEY` from the `.env` file.
- **Configure Model:** Sets up the `models/gemini-embedding-001` model.
- **Embed Content:** The `genai.embed_content()` function takes the text and converts it into a 3072-dimension vector embedding.
- **Print Results:** The code prints the generated embedding and confirms its dimension.
- **List Models:** The script also iterates through and lists all available embedding models provided by the Gemini API.
