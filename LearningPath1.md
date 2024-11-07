# Topics

## Python basics
### Concepts

### Learning Material

### Exercise

## Package management
### Concepts
1. pip
2. Creating virtual environment
3. poetry
### Learning Material
Text: 
For Poetry installation follow : https://python-poetry.org/docs/#installing-with-the-official-installer
Video: 
For Poetry windows installation - https://www.youtube.com/watch?v=5lioBm8f324

### Exercise

## Web Concepts: Client, Server and API
### Concepts

## FastAPI 
### Concepts
1. Creating a basic app which responds to GET request
2. Types, type hints and Pydantic models
3. Path and path operations
4. Response model
5. Routers (including prefix)
6. Dependency injection
7. Lifespan events
  
### Learning Material
Text: https://fastapi.tiangolo.com/learn/ (Fast API docs)
Video:
Routers - https://www.youtube.com/watch?v=D-3JJLpECGQ

### Exercise
Build a simple FastAPI app which satisfies the following conditions
1. The base url should return {"Hello":"World"}
2. When the user visits the route /v1/languages , it should return `{"languages":["en", "hi"]}`. This route should be in a separate file called languages.py and not in the main file i.e. main.py (Hint: Use routers)
3. The overall folder structure should be as follows
```
├── core
│   ├── __init__.py
│   ├── api
|   |   ├── languages.py
|   |   ├── __init__.py
├── main.py
├── venv
├── pyproject.toml
└── .gitignore
```

## Databases and ORM (SQLite and SQLAlchemy)
### Concepts
1. Database fundamentals - Relational vs NoSQL databases
2. What is SQLite and Installation (https://www.sqlitetutorial.net/what-is-sqlite/)
3. Sorting and Filtering data using SQL
4. CRUD Operations using SQL (including create, insert, update, delete, replace)
5. ORM (understanding difference b/w orm and raw sql)
6. SQLAlchemy Engine and Session
7. Transactions and Operations (including read, write, commit, rollback)
8. Metadata, Table and Column (including what is metadata, column datatypes like Integer, String)
9. Working with data using SQLAlchemy ORM (including insert, select, update, delete)
    
### Learning Material
Text
1. https://www.sqlitetutorial.net/
2. https://docs.sqlalchemy.org/en/20/tutorial/
   
### Exercise
##### Level 1
Build a FastAPI app which connects to a SQLite database named db. Create a model called Transcription, which has the following fields : id (integer), user_id(integer), transcription(string), processed_text(string), word_count(integer), language(string). The word_count field must have a default value of zero, and the language column must have a value. Create an endpoint /v1/transcriptions, which returns all the transcriptions. Create another endpoint /v1/transcriptions/save , where user can pass user_id and language, and that entry gets added to the SQLite database. Try to use dependency injection to start the SQLalchemy session

## Asynchronous Python (including Asynchronous SQLAlchemy)
Note: This is a hard topic, so if you are not able to grasp this fully, just go ahead, and you can come back to it at a later point of time
### Concepts
1. Event Loop
2. Coroutines, Asyncio, Async and Await
3. Making SQLAlchemy code asynchronous (Refer https://www.youtube.com/watch?v=cH0immwfykI)

### Exercise
Convert the FastAPI app created in the Databases and ORM section from synchronous to asynchronous. 

## Websockets
### Concepts


### Learning Material
1. https://apmonitor.com/dde/index.php/Main/WebSocketTransfer

### Exercise
#### Level 1
Complete the activity shown in https://apmonitor.com/dde/index.php/Main/WebSocketTransfer
#### Level 2



## Redis
### Concepts

### Learning Material

### Exercise

## Uvicorn
### Concepts

### Learning Material

### Exercise

## LLM and Prompt engineering
### Concepts
1. LLM basics
2. Calling LLM apis like OpenAI and Bhashini
3. Zero shot, Few shot prompting
### Learning Material
Text:

### Exercise

# Capstone Project 
This capstone project is based on a real world open source project, which you can contribute to once you finish the capstone project

