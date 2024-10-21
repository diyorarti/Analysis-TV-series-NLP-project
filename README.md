# Analysis-TV-Series-NLP-Project

This project is an in-depth exploration of natural language processing (NLP) techniques applied to analyze TV series transcripts, particularly from the anime **Naruto**. The project was inspired by Jiffy's implementation on his YouTube channel, but several additional ideas were integrated to expand the functionality. The project includes various modules for character chatbot creation, theme classification, named entity recognition (NER), character network generation, text classification, and extracting data from web pages.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Modules](#modules)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Technologies Used](#technologies-used)
7. [Datasets](#datasets)
8. [Acknowledgements](#acknowledgements)

---

## Project Overview

This project explores several natural language processing (NLP) techniques and models to extract meaningful insights from TV series scripts, specifically the anime **Naruto**. The project includes the following features:
- Character-based chatbot using a fine-tuned LLaMA model.
- Character network generation to analyze relationships between characters.
- Theme classification using a zero-shot classifier.
- Named Entity Recognition (NER) for character identification.
- Text classification for different types of **Jutsu** (ninja techniques).

---

## Features

1. **Character Chatbot**: A chatbot that simulates a conversation with the character **Naruto**, utilizing a fine-tuned LLaMA model based on the show's dialogues.
2. **Character Network Generation**: This module identifies relationships between characters using NER and visualizes these relationships as a network graph.
3. **Theme Classification**: Identifies recurring themes in the series using zero-shot classification techniques.
4. **Text Classification**: Classifies different types of **Jutsu** (ninja techniques) from the **Naruto** series.
5. **Web Scraping**: Extracts information from web pages, such as the details of various **Jutsu**.

---

## Modules

1. **Character Chatbot**: 
   - File: `character_chatbot.py`
   - This module implements a chatbot that mimics the personality and speech patterns of **Naruto** using a fine-tuned LLaMA model.

2. **Character Network Generator**: 
   - File: `character_model.py`
   - Generates a graph of relationships between characters based on their dialogue interactions using NER techniques.

3. **Named Entity Recognizer (NER)**: 
   - File: `name_entity_model.py`
   - Uses Spacy’s transformer model to identify named entities (characters) in the scripts.

4. **Text Classification (Jutsu Classifier)**: 
   - File: `jutsu_classifier.py`
   - Classifies different types of **Jutsu** techniques using a HuggingFace transformer model.

5. **Theme Classification**: 
   - File: `theme_classifier.py`
   - Uses zero-shot classification to identify themes in the TV series script.

6. **Web Scraping (Jutsu Webpage Extractor)**: 
   - File: `jutsu_webpage_extractor.py`
   - Extracts detailed information about **Jutsu** techniques from the **Naruto** fandom website.

7. **App Interface**: 
   - File: `app.py`
   - A Gradio interface that integrates all the above modules into a user-friendly application.

---

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/Analysis-TV-series-NLP-project.git
   cd Analysis-TV-series-NLP-project
2. Install dependencies: Create a virtual environment (optional but recommended):
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows, use `env\Scripts\activate`
   ```
   Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the datasets:

Naruto Season 1 Subtitle. 
```bash
https://subtitlist.com/subs/naruto-season-1/english/2206507
```
Naruto Episode 1 Transcript
```bash
https://www.kaggle.com/datasets/leonzatrax/naruto-ep-1-transcript
```


Technologies Used
Python
Gradio: For creating a web-based interface.
Transformers (HuggingFace): For chatbot and text classification models.
Spacy: For named entity recognition (NER).
Scrapy: For web scraping.
PyTorch: For model training and inference.
Pandas: For data handling and manipulation.
NetworkX: For graph-based character network generation.
Pyvis: For network visualization.








