# Mobile Application for Call Center Agents - Chatbot for Family Planning

This project is a Chatbot web application designed for the IEM-run Shukhi Poribar national call center under the Directorate General of Family Planning (DGFP), Bangladesh. The chatbot aims to assist call center agents in efficiently managing public queries related to family planning by providing accurate and timely information in Bangla.

Developed under USAID's 'Breakthrough ACTION' project in collaboration with Johns Hopkins Center for Communication Programs (JHUCCP), the chatbot is intended to improve the efficiency of health communication and service delivery.

## Background

The 'Breakthrough ACTION' initiative, spanning from December 1, 2023, to April 30, 2025, focuses on strengthening health systems and promoting effective Social and Behavior Change (SBC) communication in Bangladesh. To support this effort, a Chatbot has been developed to assist the Shukhi Poribar call center agents in handling a high volume of daily calls by providing a pre-set question-and-answer bank for frequently asked questions (FAQs).

## Key Features

- **Conversational AI in Bangla:** Provides responses to user queries in Bangla, helping call center agents handle public queries more effectively.
- **Comprehensive Question Bank:** Developed based on the 400+ page Family Planning manual, featuring categorized and segmented topics for efficient response retrieval.
- **User-Friendly Interface:** Designed with a responsive UI/UX for easy navigation and interaction by call center agents.
- **Automatic Knowledge Base Updates:** Supports seamless updates to the chatbot's knowledge base when the manual content is revised.
- **Integration with Existing Systems:** Integrates with the existing call center software and the Management Information System (MIS) of DGFP.
- **Multilingual Support:** Primary focus on Bangla, with the capability to extend to other languages.
- **Training and Support:** Includes training for agents and detailed documentation to ensure smooth usage.

## Folder Structure

The project's main folders are organized as follows:

- `/data`: Contains the `intents.json` file, which manages chatbot intents and responses.
- `/models`: Holds the pre-trained TensorFlow model file (`chatbot_model.h5`).
- `/auth`: Manages user authentication logic, including signup, login, and verification.
- `/api`: Contains Flask routes for chatbot queries and user authentication.
- `/scripts`: Includes TensorFlow model training scripts for updating the chatbot's knowledge base.
- `/docs`: Documentation folder with user manuals, technical documentation, and data flow diagrams.

## Scope of Work

The development process covered the following tasks:

1. **Needs Assessment:**
   - Conducted meetings with the IEM unit and call center agents to gather a comprehensive understanding of public queries.
   - Prepared a detailed question bank based on frequently asked questions.
2. **Design and Development:**
   - Designed a user-friendly UI/UX based on the approved question bank.
   - Developed a web application supporting multilingual responses with a primary focus on Bangla.
   - Incorporated information from the Family Planning manual into the chatbot's knowledge base.
3. **Integration:**
   - Integrated the chatbot with existing call center software and DGFP's MIS.
4. **Categorization and Segmentation:**
   - Implemented mechanisms for categorizing and segmenting specific topics for efficient response retrieval.
5. **Testing and Quality Assurance:**
   - Conducted thorough testing to ensure accuracy and reliability, incorporating feedback from IEM and Breakthrough ACTION teams.
6. **Training and Documentation:**
   - Provided training sessions for call center agents and IEM unit focal persons.
   - Created user manuals, technical documentation, and training videos.
7. **Support and Maintenance:**
   - Offered post-deployment support and maintenance for a specified period.




## Deliverables

The following deliverables were provided:

1. **Chatbot Application:**
   - A functional web application for call center agents with a categorized question-and-answer bank.
2. **Documentation:**
   - User manual, technical documents, and data flow diagrams.
   - Audio-visual guide for chatbot usage.
3. **Credentials:**
   - Handover of all credentials to the USAID 'Breakthrough ACTION' project.





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

Login Page
![Login](https://github.com/user-attachments/assets/392e6d2f-6fe2-41e4-a9e4-5ac8274a61d3)
Sign-In Page
![singin](https://github.com/user-attachments/assets/213e2104-201c-4277-ac9d-07ccf193ae33)
Home Page
![home](https://github.com/user-attachments/assets/42eaa412-586a-4e65-a003-bf9e3540ad24)
Message 
![starting_msg](https://github.com/user-attachments/assets/6375dab5-c800-4ea1-b05a-d09c1d2c963b)
Reply
![reply](https://github.com/user-attachments/assets/b52c8451-8a40-4ffa-8674-6c6b0e45ee66)






