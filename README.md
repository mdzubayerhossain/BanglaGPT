**Bangla Chatbot with GPT-like Functionality
This repository hosts a chatbot designed to mimic the functionality of ChatGPT, but specifically for Bangla. The system features user authentication, including a login/signup section with verification, and serves intelligent responses in Bangla across various topics.

Key Features:

ChatGPT-like Experience in Bangla: Provides conversational AI capabilities similar to ChatGPT, tailored for Bangla speakers.
Flask Backend: Powers the chatbot's API and user interactions with a lightweight server.
User Authentication: Implements a secure login/signup process with verification to manage user access.
Pre-Trained TensorFlow Model: Utilizes an LSTM-based TensorFlow model for natural language understanding and conversation in Bangla.
NLTK Processing: Handles tokenization, word lemmatization, and intent prediction to comprehend user queries and generate appropriate responses.
Healthcare Data Focus: Originally trained on healthcare data, offering specialized knowledge in this domain.
React Frontend Integration: Designed to work with a React frontend for a smooth user interface.
Intent-Based Response: Leverages a JSON-based intents file for handling different user queries and mapping them to correct responses.
Folder Structure:

/data: Includes the intents.json file for managing chatbot intents and responses.
/models: Contains the pre-trained model file (chatbot_model.h5).
/auth: Manages the authentication logic, including signup, login, and verification.
/api: Flask routes for handling chatbot queries and user authentication.
/scripts: Model training scripts using TensorFlow for updating the chatbot's understanding.
**
# Getting Started
To get started with this project, follow these steps:
1. Clone this repository to your local machine.
```
git clone https://github.com/mdzubayerhossain/BanglaGPT.git
```
2. Install the required Python libraries using:
```
pip install -r requirements.txt
```
3. Train the model using:
```
python training.py
```
4. Established Database connection with mysql using:
```
CREATE DATABASE IF NOT EXISTS `user-system`;
USE `user-system`;

CREATE TABLE `user` (
  `userid` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(100) NOT NULL,
  `email` varchar(100) NOT NULL,
  `password` varchar(255) NOT NULL,
  PRIMARY KEY (`userid`),
  UNIQUE (`email`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;


```
5. Final step: Run this app ->>>
```
flask run
```



