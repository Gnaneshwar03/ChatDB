# ChatDB: Q&A and RAG with SQL and Tabular Data

This project implements a versatile chatbot interface that supports question-answering (Q&A) and Retrieval-Augmented Generation (RAG) using SQL databases and tabular data. It leverages Gradio for the user interface and integrates various AI and database technologies for efficient information retrieval and processing.

## Sample Image

![image](https://github.com/Gnaneshwar03/ChatDB/assets/107243397/c5bc1aa5-b8e0-4897-89ad-e86891bfa15a)

![image](https://github.com/Gnaneshwar03/ChatDB/assets/107243397/a815fc06-babd-4d29-b653-4d00ae97af4a)

## Features

- Interactive chat interface with support for multiple functionalities
- Q&A capabilities using stored SQL databases
- RAG functionality with ChromaDB for efficient information retrieval
- Support for uploading and processing CSV/XLSX files
- Integration with Google's Generative AI for embeddings
- Flexible chat types to accommodate different data sources and query methods

## Technologies Used

- Python
- Gradio
- LangChain
- SQLAlchemy
- ChromaDB
- Google Generative AI
- SQLite

## Setup and Installation

1. Clone the repository:
   ```
   git clone https://github.com/Gnaneshwar03/ChatDB
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Set up environment variables:
   Create a `.env` file in the project root and add necessary API keys and configurations.

4. Prepare the database:
   - For stored SQL databases, ensure your `.sql` files are in the correct directory.
   - For CSV/XLSX data, run the preparation script:
     ```
     python src/prepare_csv_xlsx_sqlitedb.py
     ```

## Usage

Run the main application:

```
python app.py
```

This will launch the Gradio interface where you can:
- Choose between different chat types (Q&A with SQL, RAG with ChromaDB, etc.)
- Upload CSV/XLSX files for processing
- Interact with the chatbot using natural language queries

## Project Structure

- `app.py`: Main application file with Gradio UI setup
- `utils/`:
  - `chatbot.py`: Contains the ChatBot class with core functionality
  - `upload_file.py`: Handles file uploads and processing
  - `ui_settings.py`: UI configuration settings
  - `load_config.py`: Loads application configurations
