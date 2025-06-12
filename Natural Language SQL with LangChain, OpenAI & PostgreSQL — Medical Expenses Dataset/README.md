# Natural Language SQL with LangChain, OpenAI & PostgreSQL — Medical Expenses Dataset

## Project Overview

This project enables natural language querying over a structured dataset (medical insurance expenses) by leveraging LangChain, OpenAI, and a local PostgreSQL database. Instead of writing SQL manually, users can ask questions like:
- “What is the average charge for smokers?”

LangChain translates the question to SQL, queries the PostgreSQL database, and returns the result — all from a Jupyter Notebook interface. No backend web server (like FastAPI) is needed for this version.
This is perfect for showcasing how LLMs can bridge the gap between data science and end users in real-world analytics workflows.  

## Tools & Technologies Used

| Tool/Library         | Purpose                                                        |
| -------------------- | -------------------------------------------------------------- |
| **PostgreSQL**       | Local relational database for storing medical expenses         |
| **Pandas**           | Load and manipulate CSV data                                   |
| **SQLAlchemy**       | Interface between Python and PostgreSQL                        |
| **LangChain**        | Translate natural language into SQL                            |
| **OpenAI (GPT-4)**   | Language model that powers the natural language understanding  |
| **dotenv**           | Securely manage API keys and environment variables             |
| **Jupyter Notebook** | Interactive development environment to run the entire pipeline |

## Dataset 
**CSV File: insurance.csv**  
Fields:
- age
- sex
- bmi
- children
- smoker
- region
- charges

### Step 1: Create you table in your **LOCAL** PostgreSQL Database - using SQL

