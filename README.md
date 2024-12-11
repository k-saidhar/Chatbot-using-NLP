# Chatbot using NLP

## Overview

This project implements a chatbot using Natural Language Processing (NLP) techniques. The chatbot is designed to understand user intents and provide appropriate responses based on predefined patterns and responses. It utilizes the `nltk` library for natural language processing, `scikit-learn` for machine learning, and `streamlit` for creating an interactive web interface.

---

## Features

- **User Intent Recognition**: Understands various user intents such as greetings, farewells, gratitude, and more.
- **Response Generation**: Provides relevant responses based on user input.
- **Conversation History**: Maintains a conversation history that can be viewed by the user.
- **Interactive Web Interface**: Built using Streamlit for an easy-to-use chatbot interface.
- **Machine Learning Integration**: Uses scikit-learn to classify intents and generate responses.
- **Customizable**: Add or modify user intents via a simple JSON configuration file.

---

## Technologies Used

- **Python**: Main programming language.
- **NLTK**: Used for natural language processing (tokenization, stemming, etc.).
- **Scikit-learn**: Machine learning library for intent classification.
- **Streamlit**: Framework for building the chatbot’s web interface.
- **JSON**: Format for defining chatbot intents (patterns and responses).

---

## Installation

### 1. Clone the Repository

Clone this repository to your local machine:

```bash
git clone <repository-url>
cd <repository-directory>
```

2. Create a Virtual Environment (Optional but Recommended)

It’s recommended to create a virtual environment for managing dependencies:

```bash
Copy code
python -m venv venv
source venv/bin/activate # On Windows use `venv\Scripts\activate` 3. Install Required Packages
```

Install the required Python packages from the requirements.txt file:

```bash
Copy code
pip install -r requirements.txt 4. Download NLTK Data
```

To ensure that the NLTK library functions correctly, you need to download the necessary datasets:

```bash
python
Copy code
import nltk
nltk.download('punkt')
```

Usage
To run the chatbot application, use the following command:

```bash
Copy code
streamlit run app.py
```

Once the application is running, open the provided local URL in a web browser to interact with the chatbot. Type your message in the input box and press Enter to see the chatbot's response.

Intents Data
The chatbot’s behavior is governed by the intents.json file, which defines various user intents (tags), input patterns, and corresponding responses. You can modify this file to add new intents or adjust existing ones. Example of the file structure:

```bash
json
Copy code
{"tag": "greeting",
    "patterns": [
      "Hi",
      "How are you",
      "Is anyone there?",
      "Hello",
      "Whats up"
    ],
    "responses": [
      "Hi , i am your paramedic assistant"
    ],
    "context_set": ""
  }
```

Conversation History
The chatbot saves each interaction to a CSV file (chat_log.csv). You can view the conversation history through the sidebar on the Streamlit interface.

Contributing
Contributions to this project are welcome! If you have suggestions for improvements or features, feel free to:

Fork the repository.
Create a new branch.
Make your changes and submit a pull request.
If you find any issues, please open an issue or contribute a fix.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
NLTK: For natural language processing capabilities (tokenization, stemming, etc.).
Scikit-learn: For machine learning algorithms used in intent classification.
Streamlit: For creating the web interface of the chatbot.
OpenAI: For inspiration and example workflows.
Replace <repository-url> and <repository-directory> with the actual URL of your repository and the directory name on your system where the project resides.

Troubleshooting
If you face any issues running the project, consider checking the following:

Ensure that all dependencies are installed correctly.
Ensure that NLTK data is downloaded successfully.
Ensure you have access to the necessary API keys (if any).
markdown
Copy code

### Key Changes:

- **Clarified Structure**: The instructions are organized in a clear sequence of steps for cloning, setting up, and running the chatbot project.
- **Replaced Placeholder**: Replaced `<repository-url>` and `<repository-directory>` with a general instruction to modify them with real details.
- **Usage Details**: Emphasized usage steps for the Streamlit interface.
- **Contributing Section**: Simplified and emphasized easy contribution steps for GitHub collaboration.

This version provides a clean and easily navigable README for your GitHub project.
