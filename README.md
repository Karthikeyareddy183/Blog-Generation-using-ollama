
# Blog Generation using Ollama

## Overview

This project is a Blog Generation System that utilizes Streamlit and Ollama to generate blog content based on user input. It leverages the gemma:2b model and external resources like Wikipedia and DuckDuckGo search to enhance content generation.

## _Features_

- _Blog Generation_: Generates a blog with the following sections:
  - Heading
  - Introduction
  - Content
  - Summary
- _Research Tools_: Uses DuckDuckGo Search and Wikipedia to gather information.
- _Streamlit Interface_: Provides a simple web interface for users to input a topic and view the generated blog.
- _Download Option_: Allows users to download the generated blog as a .txt file.

---

## _Requirements_

To run this project, you need the following:

1. _Python 3.8 or later_
2. _Ollama_: A lightweight framework for running large language models locally.
3. _Streamlit_: For the web interface.
4. _LangChain_: For integrating the language model and tools.
5. _Additional Libraries_: duckduckgo-search, wikipedia-api, etc.

---

## Installation and Setup

### Step 1: Install Ollama

Download and install Ollama from the official website: [Ollama](https://ollama.com/).

### Step 2: Pull the Gemma Model

Run the following command to download the gemma:2b model:

bash

```
ollama pull gemma:2b
```

### Step 3: Install Required Libraries

Install the necessary Python dependencies using pip:

bash

```
pip install streamlit langchain langchain-community duckduckgo-search wikipedia-api
```

## Running the Project

### Start the Ollama Server

Ensure the Ollama server is running in the background before launching the application:

bash

```
ollama serve
```

### Run the Streamlit App

Navigate to the project directory and run the Streamlit app using:

bash

```
streamlit run app.py
```

### Use the App

1. Open the URL displayed in the terminal (usually [http://localhost:8501](http://localhost:8501)).
2. Enter a blog topic in the input field and click _Generate Blog_.
3. View the generated blog and download it using the _Download Blog_ button.

## Project Structure

```
Blog-Generation-using-ollama/
├── app.py # Main Streamlit app code
├── README.md # Project documentation
└── requirements.txt # List of dependencies
```

## License

This project is open-source and available under the [MIT License](LICENSE).

## Contributing

Feel free to contribute by submitting pull requests or reporting issues.
