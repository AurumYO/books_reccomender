# Books Semantic Recommender

A semantic book recommendation system built with Python, OpenAI, LangChain, and Gradio.
Bbased on online tutorial from Freecodecamp (https://www.youtube.com/watch?v=Q7mS1VHm3Yw&t=5977s)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)

## Introduction

This project provides a semantic book recommendation system that leverages advanced natural language processing techniques to suggest books based on user input. The system is built using:

- Python: The core programming language.
- OpenAI: For embeddings and language models.
- LangChain: To manage language model interactions.
- Gradio: For creating an interactive web-based user interface.

## Features

Semantic Search: Finds books that semantically match user queries.
Category Filtering: Allows filtering recommendations by book categories.
Emotional Tone Filtering: Filters recommendations based on the desired emotional tone.

## Installation

Ensure you have Poetry installed for dependency management.

Clone the Repository:

```bash
git clone https://github.com/AurumYO/books_reccomender.git
cd books_reccomender
```

### Install Dependencies:

Run the following command to install the required packages:

```bash
poetry install
```

This will create a virtual environment and install all dependencies specified in pyproject.toml.

### Set Up Environment Variables:

Duplicate the .example.env file and rename the copy to .env.
Fill in the necessary environment variables in the .env file.

## Usage

### To launch the Gradio dashboard, execute:

```bash
poetry run python gradio-dashboard.py
```

This command will start the application, and you can interact with the recommender system through the Gradio interface.

## Project Structure

```bash
books_reccomender/
├── .example.env # Example environment variables file
├── .gitignore # Git ignore file
├── README.md # Project README
├── books_cleaned.csv # Dataset of cleaned book information
├── books_with_categories.csv# Dataset with book categories
├── books_with_emotions.csv # Dataset with book emotions
├── cover_not_found.jpg # Placeholder image for missing book covers
├── data-exploration.ipynb # Jupyter notebook for data exploration
├── gradio-dashboard.py # Main application script
├── poetry.lock # Poetry lock file
├── pyproject.toml # Poetry project configuration
├── semantic-analysis.ipynb # Jupyter notebook for semantic analysis
├── tagged_description.txt # Text file with tagged book descriptions
├── text-classification.ipynb# Jupyter notebook for text classification
└── vector-search.ipynb # Jupyter notebook for vector search
```
