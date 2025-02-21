# **GenAI Builder**

## **Overview**
GenAI Builder is an AI-powered application that helps users search and retrieve the information they need efficiently. This application leverages OpenAI's API to provide intelligent responses based on user queries.

## **Setup & Installation**

### **Prerequisites**
Ensure you have the following installed on your system:
- **Docker** ([Install Docker](https://www.docker.com/get-started))

### **1. Get an OpenAI API Key**
1. Go to [OpenAI API Keys](https://platform.openai.com/settings/organization/api-keys).
2. Generate an API key.
3. Create a `.env` file inside the project directory and add the following:
   ```plaintext
   OPENAI_API_KEY=your_api_key_here
   ```

## **🚀 Running the Application Using Docker**

### **1. Build the Docker Image**
```bash
docker build -t genaidemo .
```

### **2. Run the Container**
```bash
docker run -p 8080:5000 genaidemo
```

### **3. Access the Application**
- Open your browser and go to:
  ```
  http://localhost:8080
  ```

## **📂 Project Structure**
```
📦 genai-builder
├── 📄 Dockerfile
├── 📄 .env (Add API Key here)
├── 📄 app.py (Main application logic)
├── 📄 requirements.txt (Dependencies)
├── 📂 templates (HTML templates)
└── 📄 README.md (You are here)
```

## **🛠️ Troubleshooting**
- **Issue:** API key not found  
  **Solution:** Ensure the `.env` file exists and contains a valid API key.
- **Issue:** Port conflict on `8080`  
  **Solution:** Change the port mapping in the `docker run` command:
  ```bash
  docker run -p 9090:5000 genaidemo
  ```

## **🙌 Contributing**
Feel free to open **issues** or **pull requests** to enhance the functionality!

---

**Happy Building! 🚀**

