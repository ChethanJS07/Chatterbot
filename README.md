# Python Chatbot with Knowledge Base

This Python script implements a simple chatbot that interacts with users based on predefined questions and answers stored in a JSON knowledge base file.

## Features

- **Loading and Saving Knowledge Base:** Utilizes JSON files to store and retrieve a collection of questions and answers.
- **Matching User Input:** Uses the `difflib.get_close_matches` function to find the closest match to user queries.
- **Dynamic Learning:** Allows the chatbot to learn new responses from users for questions it doesn't already know.

## Requirements

- Python 3.x
- `json` module (standard library)
- `difflib` module (standard library)

## Installation

No special installation steps required. Ensure Python 3.x is installed on your system.

## Usage

1. **Setup:**
   - Create a `knowledge_base.json` file with initial questions and answers in the following format:
     ```json
     {
       "questions": [
         {"question": "What is your name?", "answer": "I am a chatbot."},
         {"question": "How old are you?", "answer": "I don't have an age."},
         ...
       ]
     }
     ```

2. **Execution:**
   - Run the script `chatbot.py`.
   - Enter queries to interact with the chatbot. Type `quit` to exit.

3. **Learning:**
   - If the chatbot doesn't know an answer, it asks for user input to learn a new response.
