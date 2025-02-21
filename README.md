GenAI Builder
This application builds a GenAI-powered search tool that helps users retrieve the information they need efficiently.

🔧 Setup & Installation
1. Prerequisites
Ensure you have the following installed on your system:

Docker (Install from here)
2. Get an OpenAI API Key
Go to OpenAI API Keys.

Generate an API key.

Save it in a .env file inside the project directory:

plaintext
Copy
Edit
OPENAI_API_KEY=your_api_key_here
🚀 Run the Application Using Docker
Build the Docker Image

bash
Copy
Edit
docker build -t genaidemo .
Run the Container

bash
Copy
Edit
docker run -p 8080:5000 genaidemo
Access the Application

Open your browser and go to:
arduino
Copy
Edit
http://localhost:8080
📂 Project Structure
scss
Copy
Edit
📦 genai-builder
├── 📄 Dockerfile
├── 📄 .env (Add API Key here)
├── 📄 app.py (Main application logic)
├── 📄 requirements.txt (Dependencies)
├── 📂 templates (HTML templates)
└── 📄 README.md (You are here)
🛠️ Troubleshooting
Issue: API key not found
Ensure .env file exists and contains a valid API key.
Issue: Port conflict on 8080
Change the port mapping in the docker run command:
bash
Copy
Edit
docker run -p 9090:5000 genaidemo
