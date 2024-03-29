# chitti_thechatbot
## E-commerce chat bot using Rasa framework
This Rasa chatbot serves as a smart chatbot speaking to people and educating/informing them about Ecommerce search assistant. We are making API calls to https://fakestoreapi.com/products to get products and categories from Action server.
## Files in Rasa Folder
A brief rundown of the purpose of some of the files, which are closely interconnected with one another.

#### actions.py 
This file contains all written Python code of custom actions.

#### config.yml 
This file contains configurations for Rasa NLU and Rasa Core, such as tokenizers and policies.

#### credentials.yml
This file contains the credentials for the voice & chat platforms which the bot is using.

### data :

#### nlu.yml
This file contains all the intents and their variations.

#### stories.yml
This file contains different variations of paths that a user might go through.

#### rules.yml 
This file is a new addition from Rasa v1.x, containing the rules that define certain conversational paths of the chatbot

#### domain.yml
This file contains the actions, utters, entities, forms, slots, responses and buttons that are used.

#### endpoints.yml
This file contains the different endpoints the bot can use.

#### models
This folder contains model(s) which are trained.
## Installation
Rasa Quick Installation

You can install Rasa Open Source using pip. It is strongly recommended to create a virtual environment.

To create a virtual environment, check out this video : https://www.youtube.com/watch?v=hqkfHK7-O08

For full installation guide, check out the Rasa Documentation(https://rasa.com/docs/rasa/installation/).

### Installing rasa framework(use the following code)
pip install rasa

## Running locally
The bot can be run on Terminal locally. The bot calls the action server via the url specified under endpoints.yml.

### 1. Run Rasa Shell In a Terminal tab in your bot directory, enter this command line to run rasa:
rasa shell
### 2. Run Action Server Running the action server is necessary to utilise the custom actions writtten in actions.py. 
To run the action server, open up another tab in Terminal and enter this command line:

rasa run actions 

#### Now in the rasa shell terminal we can chat with the chatbot.
