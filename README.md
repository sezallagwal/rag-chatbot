# RAG Chatbot

A RAG Chatbot is an AI-powered conversational assistant designed to run on various platforms. It utilizes the Retrieval Augmented Generation (RAG) architecture, which combines the power of retrieval-based and generation-based language models. This chatbot is specialized in answering with given input data. It can be deployed on different devices, making it suitable for embedded and edge computing based applications.

1. AI-powered conversational assistant for various platforms.
2. Specialized in answering frequently asked questions related to different topics.
3. Utilizes Retrieval Augmented Generation (RAG) architecture to retrieve relevant information from a knowledge base.
4. Generates contextual and fluent responses based on the retrieved knowledge.
5. Deployable on different platforms for embedded and edge computing applications.

## Step 1: Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/sezallagwal/rag-chatbot/ chatbot
   cd chatbot
   ```

## Step 2: Input Data

To provide the necessary input for the chatbot, place your input data files in the `/data` folder. These files should contain the questions and answers that the chatbot will use to generate responses.

## Step 3: Docker Deployment

### Why Docker?

Docker is being used here to provide a consistent and isolated environment for running the chatbot application. It allows us to package all the necessary dependencies and configurations into a single container, making it easier to deploy and manage the application across different platforms and environments. Additionally, Docker provides a lightweight and efficient runtime, which is especially beneficial for resource-constrained devices. By using Docker, we can ensure that the chatbot application runs smoothly and consistently, regardless of the underlying system setup.

To Install Docker:

- For Ubuntu, run the following commands:

  ```bash
  sudo apt-get update
  sudo apt-get install docker.io
  ```

- For other operating systems, refer to the official Docker documentation: [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/)

1. Build the Docker image:

   ```bash
   docker build -t chatbot .
   ```

2. Run the Docker container:
   ```bash
   docker run -d -p 8501:8501 chatbot
   ```

## Step 4: Access the Chatbot

Once the Docker container is running, you can access the chatbot by navigating to:

```bash
http://localhost:8501
```
