# GPT-3 Sentiment Analysis Project

## Project Description
This project is an interactive Python application that engages users in a conversation, generates responses using OpenAI's GPT-3 model, performs sentiment analysis on those responses, and creates visual reports summarizing the sentiment analysis results. The project integrates with a PostgreSQL database to store and retrieve conversation data and supports Docker deployment for easy setup and sharing.

## Features
- **User Interaction**: Allows multiple interactions with users, providing a conversational experience.
- **GPT-3 Text Generation**: Uses OpenAI's GPT-3 model to generate responses based on user input.
- **Sentiment Analysis**: Analyzes the sentiment of generated responses, classifying them as positive, negative, or neutral.
- **Data Visualization**: Generates visual reports, including pie charts, to represent sentiment distribution.
- **PostgreSQL Integration**: Stores conversation data in a PostgreSQL database for persistence and retrieval.
- **Docker Deployment**: Provides a Dockerfile for easy containerization and deployment.

## Dependencies
The project relies on the following Python packages:
- `openai`: For interacting with OpenAI's GPT-3.
- `textblob`: For sentiment analysis.
- `matplotlib`: For data visualization.
- `psycopg2`: For PostgreSQL database integration.

Ensure you have Python 3.7 or later installed to run the project.

## Setup Instructions
### Install Dependencies
If not using Docker, install the required packages with:

```bash
pip install openai textblob matplotlib psycopg2
```

### OpenAI API Key
Set your OpenAI API key as an environment variable or replace `your-api-key-here` with your key in the code. This key is required to interact with GPT-3.

### PostgreSQL Setup
Ensure you have PostgreSQL installed. Create a database named `sentiment_db` and set environment variables for connection details:

```bash
export DB_HOST='localhost'
export DB_PORT='5432'
export DB_USER='your_db_user'
export DB_PASSWORD='your_db_password'
export DB_NAME='sentiment_db'
```

### Run the Application
If not using Docker, run the Jupyter Notebook or Python script to interact with the application:

```bash
jupyter notebook
```

Open the Jupyter Notebook and follow the code cells to interact with GPT-3, analyze sentiment, and generate data visualizations.

### Docker Deployment
To deploy the project using Docker, follow these steps:

1. **Build the Docker Image**:
   ```bash
   docker build -t gpt3-sentiment .
   ```

2. **Run the Docker Container**:
   ```bash
   docker run -p 8888:8888 gpt3-sentiment
   ```

Open the Jupyter Notebook in your browser to interact with the application.

## Usage Instructions
### Interact with GPT-3
Start the notebook or Python script, and enter text when prompted with "You:". The application will generate a GPT-3 response, which is then displayed.

### Perform Sentiment Analysis
The application performs sentiment analysis on GPT-3 responses, classifying them as positive, negative, or neutral.

### Generate Data Visualizations
The project creates a pie chart showing the sentiment distribution, based on the analysis results.

## Contact Information
For any questions or issues, please contact:
- **Name**: Bidisha Biswas
- **Email**: bidisha1704@gmail.com
- **LinkedIn**: https://www.linkedin.com/in/bidisha-biswas/

## Acknowledgments
Special thanks to OpenAI for providing the GPT-3 model and to the contributors of the Python libraries used in this project.

