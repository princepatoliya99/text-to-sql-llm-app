# Text-to-SQL LLM App

An AI-powered tool that converts natural language questions into SQL queries and executes them against a database, built using Google's Gemini LLM.

## Features
- Converts plain English questions into SQL queries using Google Gemini
- Supports CSV upload, automatically converting data into a SQLite database
- Dynamically adapts to different schemas based on uploaded data
- Interactive Streamlit interface for querying and viewing results
- Automatic cleanup of temporary databases after use

## Tech Stack
- Python
- Google Gemini API
- SQLite
- Streamlit

## How It Works
1. User uploads a CSV file or uses the pre-loaded dataset
2. The app converts the file into a SQLite database and reads its schema
3. User asks a question in plain English
4. Gemini LLM translates the question into a valid SQL query based on the schema
5. The query is executed against the database and results are displayed

## Setup
1. Clone the repository
   \`\`\`bash
   git clone https://github.com/princepatoliya99/text-to-sql-llm-app.git
   cd text-to-sql-llm-app
   \`\`\`
2. Create a virtual environment and install dependencies
   \`\`\`bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   \`\`\`
3. Add your Google Gemini API key as an environment variable
4. Run the app
   \`\`\`bash
   streamlit run app.py
   \`\`\`

## What I Learned / Built
- Prompt engineering for structured output generation (natural language → SQL)
- Handling dynamic database schemas
- Integrating an LLM API into a Python application
- Building an interactive UI with Streamlit

## Author
Prince Patoliya
