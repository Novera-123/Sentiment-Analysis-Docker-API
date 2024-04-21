# Sentiment-Analysis-Docker-API

elcome to the Text Classification API repository! This API utilizes a pre-trained Hugging Face Transformer model to perform sentiment analysis on text. It's built using FastAPI and containerized with Docker for easy deployment and scalability.

## Features
- Sentiment Analysis: Analyze text to determine if the sentiment is positive, negative, or neutral.
- FastAPI Framework: Fast and robust API framework with automatic interactive API documentation.
- Docker Integration: Containerized application for straightforward setup and deployment.

## Prerequisites
Before you begin, ensure you have Docker installed on your machine. If you don't have Docker yet, you can download it from Docker Hub.

## Getting Started
Clone the Repository
Start by cloning this repository to your local machine:

```bash
# Clone the repository
git clone https://github.com/your-github-username/text-classification-api.git
cd text-classification-api'''

# Build the Docker container
docker build -t text-classification-api .

bash
Copy code
docker build -t text-classification-api .
Run the Container
Once the build is complete, you can run the container:

bash
Copy code
docker run -p 8000:8000 text-classification-api
Access the API
The API is now running at http://localhost:8000. You can interact with the API directly or use the automatic documentation provided by FastAPI at http://localhost:8000/docs for a more interactive experience.

API Endpoints
GET /: A simple welcome message to ensure the API is operational.
POST /analyze: Endpoint to analyze the sentiment of provided text. Accepts JSON input containing a "text" field.
Example request for /analyze endpoint:

json
Copy code
{
  "text": "I love this product!"
}
Running Tests
To run automated tests for the API, execute the following command:

bash
Copy code
pytest
These tests check the functionality of the API endpoints to ensure they handle both expected and edge cases correctly.

## Documentation
The API documentation is automatically generated by FastAPI and is available at http://localhost:8000/docs. This includes detailed information about the endpoints, expected input, and formats.

## Deployment
For instructions on deploying this API to Hugging Face Spaces or other environments, refer to the provided deployment guidelines in this repository.

## Contributing
Feel free to fork this repository and submit pull requests to contribute to its development. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the apache License - see the LICENSE file for details.
