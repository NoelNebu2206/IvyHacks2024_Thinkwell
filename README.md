# ThinkWell AI: Mental Health Companion

ThinkWell AI is an advanced mental health support application designed to offer therapeutic assistance through Cognitive Behavioral Therapy (CBT) techniques. Leveraging a FastAPI backend integrated with various machine learning models and services, ThinkWell AI provides real-time, personalized mental health support. Users interact with the ThinkWell AI chatbot via a friendly web interface powered by Streamlit, ensuring an engaging conversational experience.

## Features

- **Personalized Therapy Sessions**: Users receive therapy sessions tailored to their needs, facilitated by an AI therapist named "Thinkwell."
- **Real-time Interaction**: The application utilizes the Cohere Chatbot and RagChain models to process and respond to user inputs dynamically, simulating a natural conversation flow.
- **Session Management**: Users can start, continue, and end sessions, with all interactions securely logged for continuity of care.
- **User Authentication**: Secure Google OAuth authentication ensures that only authorized users can access their sessions.
- **Responsive Design**: The application is designed to be responsive and accessible from various devices, ensuring a seamless user experience.

## Technologies Used

- **FastAPI**: Builds the robust API that handles all backend logic, including user data processing and session management.
- **Streamlit**: Provides the frontend interface for user interaction with the AI chatbot.
- **MongoDB Atlas**: Secures the storage of user sessions and transcripts, ensuring data persistence and security.
- **Cohere Chatbot**: Powers AI-driven responses, offering a conversational model that handles user queries in real-time.
- **RagChain**: Integrates multiple data sources for comprehensive context management during user interactions.
- **Modal**: Hosts the FastAPI server serverlessly.

## How to Run the Application

### Setup Environment

1. Ensure Python 3.8 or newer is installed.
2. Install required packages from the provided `requirements.txt` file using the command:
   ```sh
   pip install -r requirements.txt

### API Keys and Authentication

1. Set up Google OAuth credentials and MongoDB Atlas for database management.
2. Ensure all secret keys and API endpoints are configured correctly in the application settings.

### Starting the Server

1. Run the FastAPI server with the command:
   ```sh
    modal serve modal_back.py
   
2. Open another terminal and start the Streamlit frontend:
   ```sh
   streamlit run streamlit_app.py

### Using the Application:

1. Navigate to the specified localhost address in a web browser to interact with the ThinkWell AI chatbot.
2. Log in using a Google account to start a session.

### Security and Privacy

All user data is handled with strict confidentiality. Authentication is managed through secure protocols, and user transcripts are stored securely in MongoDB Atlas with restricted access.
