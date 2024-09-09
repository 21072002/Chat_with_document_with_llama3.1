# Llama 3.1 Document Chatbot

This project features a chatbot built using Llama 3.1 for document-based interactions. It demonstrates how to set up a virtual environment, install required libraries, configure a Groq API key, and run the chatbot application.

## Prerequisites

- Python 3.8 or higher installed on your system.

## Setup Instructions

### 1. Clone the Repository

Clone this repository to your local machine:

```bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
```

### 2. Create a Virtual Environment

Create a virtual environment to isolate your project’s dependencies:

```bash
python -m venv venv
```

Activate the virtual environment:

- **On Windows:**

    ```bash
    .\venv\Scripts\activate
    ```

- **On macOS and Linux:**

    ```bash
    source venv/bin/activate
    ```

### 3. Install Required Libraries

Install the required libraries using `pip`. Make sure you have a `requirements.txt` file that includes all the necessary dependencies:

```bash
pip install -r requirements.txt
```

If you don't have a `requirements.txt` file, you can create one by running:

```bash
pip freeze > requirements.txt
```

### 4. Set Up Your Groq API Key

Set up your Groq API key by adding it to the virtual environment:

- **On Windows:**

    ```bash
    setx GROQ_API_KEY "your-groq-api-key"
    ```

- **On macOS and Linux:**

    ```bash
    export GROQ_API_KEY="your-groq-api-key"
    ```

Alternatively, you can store the API key in a `.env` file in the root of your project and load it using the `python-dotenv` package:

1. Install `python-dotenv`:

    ```bash
    pip install python-dotenv
    ```

2. Create a `.env` file:

    ```plaintext
    GROQ_API_KEY=your-groq-api-key
    ```

3. Load the environment variable in your Python code:

    ```python
    from dotenv import load_dotenv
    import os

    load_dotenv()  # Load environment variables from .env file
    groq_api_key = os.getenv("GROQ_API_KEY")
    ```

### 5. Run the Chatbot

Run the `main.py` script to start the Llama 3.1 document chatbot:

```bash
python main.py
```

This will execute the chatbot application using the virtual environment with all necessary configurations set up.

## Additional Information

- Ensure that the `GROQ_API_KEY` is securely managed and not exposed in public repositories.
- For detailed instructions on how to interact with the Llama 3.1 chatbot or modify its behavior, refer to the `docs/` directory or the code comments in `main.py`.
- If you encounter any issues, please refer to the troubleshooting section or contact the maintainers.


### Steps to Use This README

1. **Replace placeholder text** (`your-username`, `your-repository`, `your-groq-api-key`) with actual values for your project.
2. **Ensure `requirements.txt`** is up-to-date with all the necessary dependencies for your project.

Feel free to adjust any details based on your project's specific requirements or configurations!
