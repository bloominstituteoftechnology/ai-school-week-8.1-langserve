# Week 8.1: LangServe

## Introduction
Seamlessly deploy and manage LangChain-based agents using LangServe, Docker, LangChain CLI, and Render for efficient cloud operations. [Access a LangServe scaffold made using Docker and ready to deploy on Render here.](https://github.com/bloominstituteoftechnology/ai-deployment-example)

## Prerequisites
Before you begin, ensure you have met the following requirements:
- You have installed Python 3.6+.

## Setup Instructions

### Step 1: Clone the Repository
First, clone the repository to your local machine using the following command:
```bash
git clone [repository-url]
cd [repository-name]
```

### Step 2: Create a Python Virtual Environment
Create a virtual environment using `venv`:
```bash
python3 -m venv venv
```

### Step 3: Activate the Virtual Environment
Activate the virtual environment:
- On Windows:
  ```bash
  venv\Scripts\activate
  ```
- On MacOS/Linux:
  ```bash
  source venv/bin/activate
  ```

### Step 4: Install Required Packages
Install the required packages using `pip`:
```bash
pip install -r requirements.txt
```

### Step 5: Create a `.env` File
Create a `.env` file in the root directory of the project. Use the `.env.sample` file as a reference:
```bash
cp .env.sample .env
```

### Step 6: Update `.env` File
Open the `.env` file and update the key values as necessary.

### Step 7: Export the Variables Inside Your Environment
Run the environment setup script:
```bash
export OPENAI_API_KEY=[your-key-here]
export LANGCHAIN_API_KEY=[your-key-here]
export LANGCHAIN_TRACING_V2=true
export LANGCHAIN_PROJECT=default
```

## Usage

#### Running In-Class Examples
To run any in-class examples, execute the server file directly from the command line. For example:

```bash
python3 in_class_examples/[folder]/server.py
```
After the server is running locally, you can interact with it inside `client.ipynb`.
