# CentraBot

# CentraLogic Employee Bot

## Objective
The goal is to create a bot that answers common questions related to the employee handbook, such as:
- Is it a holiday on a specific date?
- How do I request a letter from HR?
- How do I use HuHoka?

In the future, the bot will be extended to include features like:
- Bike Pool: Who all are traveling to my hometown this Friday?
- Lunch Menu: What's for lunch today?

## Technology Stack
- **Language:** Python
- **Libraries:** Langchain/LangGraph
- **Database:** Vector database for efficient query handling
- **UI:** Simple and user-friendly interface, similar to Streamlit / Chainlit, with an eventual goal to integrate into HuHoka HR

## Project Structure
  ```bash
      CentraBot/
      ├── src/
      │ ├── bot/
      │ │ ├── handlers/
      │ │ │ ├── holiday_handler.py
      │ │ │ └── hr_request_handler.py
      │ │ └── init.py
      │ ├── ui/
      │ │ ├── admin.py
      │ │ └── user.py
      │ ├── utils/
      │ │ ├── database.py
      │ │ └── vector_search.py
      │ ├── config/
      │ │ └── config.py
      │ └── app.py
      ├── README.md
      ├── requirements.txt
      ├── .env
      └── .gitignore
  ```


## Installation
- Refer to requirements.txt

### Prerequisites
- Python (3.8 or higher)
- pip (latest version)
- A vector database setup (e.g., Pinecone, Weaviate)

### Steps
1. Clone the repository:
    ```bash
    git clone https://github.com/Sakshi1261/CentraBot.git
    cd CentraBot
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv .venv
    source venv/bin/activate  
    ... # On Windows use: 
    .venv\Scripts\activate
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up environment variables:
    Create a `.env` file in the root directory and add the necessary configuration values (e.g., API keys, database URLs).

5. Run the application:
    ```bash
    python src/app.py
    ```

## Usage
- **Ask about holidays**: "Is it a holiday on [date]?"
- **Request HR documents**: "How do I request a letter from HR?"
- **HuHoka usage guidance**: "How do I use HuHoka?"

## Coding Best Practices for Python
1. **Modular Code**: Structure your code into modules for better maintainability.
2. **Environment Variables**: Store configuration and secrets in environment variables.
3. **Error Handling**: Implement proper error handling mechanisms.
4. **Testing**: Write unit and integration tests to ensure code quality.
5. **Documentation**: Maintain clear and concise documentation for your code and API endpoints.
6. **Security**: Follow best practices for security, including input validation and secure storage of sensitive data.

## Future Enhancements
- **Bike Pool Feature**: Allow employees to see who is traveling to their hometown on a specific date.
- **Lunch Menu Feature**: Display the lunch menu for the day.

## Contribution
Contributions are welcome! Please fork the repository and create a pull request with your changes. Ensure your code adheres to the project's coding standards and includes relevant tests.



Feel free to reach out to the project maintainer for any questions or support. Happy coding!
