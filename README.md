# SQL2DuckDB
This project provides a tool to convert SQL queries written in MySQL syntax to DuckDB-compatible syntax. 
## Feature
Converts MySQL queries to DuckDB with specific formatting rules trained using the Few Shot Learning Algorithm.

## Main Components
The main components of the Project are as follows:
1. Google Gemini AI API to access the latest Gemini LLM Model
2. Few Shot Learning: A technique for training LLM models where the model can understand the kind of output required for an input based on a set of IP/OP examples.
3. Vector Database: To store the example prompts effectively.
4. Langchain: A framework that helps in implementing LLM training

## How it works
1. First the model is invoked from Google using API Key from Gemini Studio
2. A custom prompt that defines the rules for conversion is mentioned
3. Few Shot examples are defined
4. The Model is invoked based on the custom prompt and the few shot examples.
5. The Output Query is formatted for better readability.

## Prerequisites
Python 3.8+
Google Cloud API Key with access to gemini-pro model
Basic knowledge of MySQL and DuckDB for SQL syntax understanding.

## Setup
1. Clone the repository:
   git clone https://github.com/yourusername/mysql-to-duckdb-converter.git
2. cd mysql-to-duckdb-converter
3. Install dependencies:
   pip install -r requirements.txt
4. Edit the main file and include the query you want to convert
5. Run the main file to get the output.

