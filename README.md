# LLM-FastAPI: AI-Powered API with FastAPI & Gemini

- LLM-FastAPI is a lightweight backend service that leverages FastAPI and Google's Gemini API to generate AI-powered responses. It provides an endpoint to interact with Gemini-Pro for text generation, making it easy to integrate LLMs into applications.

- This project also includes a React frontend to interact with the backend and is fully containerized with Docker for easy deployment.

## Important Note

- **If you face any difficulty please do checkout for the .sh file and list_of_commands.txt file in the repo**
  
## Tech Stack

- Backend: FastAPI, Uvicorn, Google Generative AI SDK

- Frontend: React.js

- Containerization: Docker & Docker Compose

- Deployment: Gitpod (or any cloud-based dev environment)

## Features

- Fast & Lightweight FastAPI backend

- AI-Powered Responses using Google's Gemini-Pro model

- CORS Enabled for seamless frontend-backend communication

- Docker Support for hassle-free deployment

## Installation & Setup

You can set up the project using either manual installation or Docker.

### Manual Installation

### Backend Setup

- Clone the repository
  
```
git clone https://github.com/gunavardhangolagani/llm-fastapi.git
cd backend
```

- Install dependencies
  
```
pip install -r requirements.txt
```

- Run FastAPI server
  
```
uvicorn main:app --host 0.0.0.0 --port 8000 --reload
```

### Frontend Setup

- Navigate to frontend directory
  
```
cd ../frontend
```

- Install dependencies
  
```
npm install
```

- Start the frontend
  
```
npm start
```

## Docker Setup

### Using Docker Compose (Recommended)

- Build and start the containers
  
```
docker compose build
```

```
docker compose up
```

### Manually Running Containers

- Backend
  
```
cd backend
```

```
docker build -t llm-backend .
```

```
 docker run -p 8000:8000 llm-backend
```

- Frontend
  
```
cd ../frontend
```

```
 docker build -t llm-frontend .
```

```
 docker run -p 3000:3000 llm-frontend
```

### API Usage

- Root Endpoint

Request:

```
GET /
```

Response:

```
{"Hello": "World,Universe"}
```
