# simple_custom_chatbot
A chatbot based on GPT-3.5-Turbo is customized in a simple way by providing a context file

### Summary
This project is about customizing a chatbot, which is based on the GPT3-Turbo model. The main idea of this project is suggested by udacity in the framework of a generative AI online course. The custom design is realized by providing context information to this model with each question the user asks the chatbot.
Our context we whish to provide the chatbot consists in a list of character descriptions from theater, television, and film productions. Each row of this list contains the name, description, medium, and setting. The list is made available by udacity and all characters were invented by an OpenAI model.
The idea of choosing a character dataset for customizing a chatbot is to study a model bias towards names and how this can be influenced by external sources.
For this purpose, we consider asking the chatbot about a likely personality and appearance of persons possessing certain names and repeat asking the chatbot the same question while providing context information about character descriptions.

### Motivation
The motivation of this project is to demonstrate in a simple way how to customize a given chatbot based on the OpenAI-GPT-3.5-Turbo model.
The customization is done by providing context information using a file in a tabular form (CSV-format).

### Data sources 
This project uses a file comprising a list of character descriptions from theater, television, and film productions. Each row of this list contains the name, description, medium, and setting. The list is made available by udacity and all characters were invented by an OpenAI model.


### Acknowledgements
The data was provided through the company "udacity" in the framework of a generative AI online course.


### Install/run instructions:
1. Install python = 3.10 and the packages denoted in requirements_working_configuration.txt preferably in a virtual environment as exemplarily shown for the windows command prompt:
```
      projectfolder:> python -m venv .venv
      projectfolder:> cd .venv\Scripts
      projectfolder\.venv\Scripts> .\activate.bat
      projectfolder\.venv\Scripts> cd ..\..
      projectfolder:> python -m pip install -r requirements.txt
```
      Within your project folder "projectfolder" use the "python" command as long as the virtual environment is activated
      (if not working with/on the project, the virtual environment should be deactivated by executing projectfolder\.venv\Scripts\deactivate.bat).

2. In the programming IDE select .venv\Scripts\python.exe as Kernel for the corresponding ipynb-file.

3. Run the ipynb-file

### Files in the repository
```
.gitignore
data
|-character_descriptions.csv         # character descriptions file
README.md
requirements.txt                     # list of packages covering a working configuration
simple_custom_chatbot.ipynb          # main Jupyter Notebook
user_key.txt                         # OpenAI API Key in UTF-8-Encoding - currently not used but can be activated by uncommenting
```
