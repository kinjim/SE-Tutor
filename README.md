**SE Tutor Application**
An interactive, AI-powered pedagogical tool built as a Jupyter Notebook application to help users master core software engineering principles through real-time tutoring and gamified assessments.  

**Features**
Multi-Engine AI Support: Seamlessly toggle between Google Gemini and OpenAI GPT-4o-mini for intelligent responses.  

Focused Learning Tracks: Targeted content for SDLC, Design Patterns, Agile/Scrum, UML, and Testing/QA.  

Intelligent Chat Tutor: A specialized persona providing concise, technical guidance limited to 5 sentences to maintain clarity.  

Dynamic Quiz Engine: Real-time generation of multiple-choice technical questions with immediate feedback and explanations.  

Gamified Progress Tracking: A built-in dashboard to monitor Experience Points (XP) and proficiency levels across engineering domains.  

**Requirements**
Environment: Google Colab or a local Jupyter Notebook instance.  

Python 3: Core execution language.  

Libraries: google-generativeai, openai, and ipywidgets.  

**How to Run**
Install Dependencies:

Bash
_pip install -q -U google-generativeai openai ipywidgets_
API Keys: Obtain a Gemini API Key from Google AI Studio or an OpenAI API Key from the OpenAI Dashboard.  

Initialize: Paste your keys into the notebook's configuration cell and run all cells to launch the interactive UI.  

**Usage**
Ask the Tutor: Use the chat interface to ask questions; responses are automatically limited to be brief and focused.  

Take a Quiz: Select a topic and click Generate Question to test your knowledge.  

Track Progress: Use the visual dashboard to view your total XP, accuracy rates, and attempt history per topic.  

**Project Structure**
SE_Tutor.ipynb: The main source file containing the UI logic, AI prompts, and state management.  

**Development and Implementation****
_Original Design Goal_
The goal was to transform a standard coding notebook into a specialized learning hub that provides more than just static text.  

**Solution Implemented**
State Management: Used a global class to track user performance data across different notebook interactions.  

Structured AI Output: Implemented strict prompt engineering to force the AI to return JSON-formatted quiz data for reliable parsing.  

Concise Tutoring: Applied system-level constraints to ensure the AI remains a focused tutor rather than a conversationalist.  

**Key Technical Challenges**
UI Integration: Leveraging IPyWidgets and IPython HTML/CSS to create a polished application interface inside a notebook.  

Reliable Parsing: Handling potential AI output errors by including cleaning logic to strip markdown formatting from JSON strings.  

**License**
This project is open source. Use as you wish.
