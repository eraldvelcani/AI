# AI — Linux Assistant using Google AI API

A lightweight AI assistant for Linux, built to help you interact with and manipulate your file and folder environment using natural language commands. 
It uses the Google AI API under the hood to interpret your intents and perform file-system operations.

---

## Features

- Interpret natural language instructions to operate on files/folders (e.g. “create folder X”, “move file Y to Z”, “delete old logs”)  
- Safeguards to prevent destructive commands without confirmation  
- Modular architecture: separate modules for prompt creation, function invocation, etc.  
- Basic testing suite to verify key functions  

---

## Contents / Project Structure
. </br>
├── calculator/ # (if present) helper arithmetic logic </br>
├── functions/ # modules containing file/folder operations </br>
├── call_function.py # code to call external functions based on intent </br>
├── config.py # configuration (e.g. API keys, paths) </br>
├── main.py # entrypoint / orchestration </br>
├── prompts.py # prompt templates, system / user prompt logic </br>
├── system_prompt # base system prompt instructions (text) </br>
├── tests.py # simple tests </br>
└── requirements.txt # Python dependencies </br>


---

## Requirements / Prerequisites

- Python 3.8+ (tested on 3.9 / 3.10)  
- A Google AI API key / credentials  
- Internet connectivity for calls to the AI service  
- Proper environment variables or config entries for API secrets  

---

## Installation & Setup

1. **Clone this repository**  
   git clone https://github.com/eraldvelcani/AI.git
   cd AI
   
2. **Install dependencies**
   pip install -r requirements.txt

3. **Configure API credentials**
   Edit config.py or set environment variables to include your Google AI API key / credentials.
   Example in config.py:
   API_KEY = "your_key_here"
   BASE_URL = "https://api.google.com/…"


(Optional) Adjust system prompt
The file system_prompt holds core instructions for the assistant. You can tailor it to your use case.

---

##Usage

Run the assistant via:
python main.py

It will prompt you (or accept commands) in natural language.


