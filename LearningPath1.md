# Topics

## Python basics
### Concepts
1. Variables
2. Data Types
3. Functions
4. Generators
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
1. Websockets vs HTTP (including lifecycle of websocket, websocket url, pros and cons of web socket)
2. Building simple websocket client server using Python websockets library
3. Using websockets in FastAPI (refer https://fastapi.tiangolo.com/advanced/websockets/)

### Learning Material
1. https://apmonitor.com/dde/index.php/Main/WebSocketTransfer
2. https://fastapi.tiangolo.com/advanced/websockets/

### Exercise
#### Level 1
Complete the activity shown in https://apmonitor.com/dde/index.php/Main/WebSocketTransfer
#### Level 2
Build a simple messaging app between multiple clients using FastAPI and websockets. You can refer to the code in FastAPI docs, but do make sure to add one additional feature of your own
#### Level 3


## Redis
### Concepts
1. Key value store (https://stackoverflow.com/questions/3046001/what-does-document-oriented-vs-key-value-mean-when-talking-about-mongodb-vs-c)
2. Installing Redis (if Windows, check out https://www.youtube.com/watch?v=DLKzd3bvgt8)
3. Redis data types (including string, hash, set, list)
4. Redis string commands (including get, set, mget, keys, exists, persist, expire)
5. Redis hash commands (including hset, hget, hmget, etc)
6. Using Redis with FastApi
### Learning Material
1. https://redis.io/learn/howtos/quick-start/cheat-sheet
2. https://www.youtube.com/watch?v=6nY-kci1rlo (Redis with FastAPI in 16mins)
   
### Exercise
#### Level 1
In the terminal/command prompt, create 2 entries with hash datatype. Then retrieve all of them
#### Level 2
Create a FastAPI app which gets data from any of the public APIs in the link - https://github.com/public-apis/public-apisand then caches it using redis, so that when the end users call the same url, they get the same data instantaneously

## LLM and Prompt engineering
### Concepts
1. LLM basics
2. Calling LLM apis like OpenAI and Bhashini
3. Zero shot, Few shot prompting
### Learning Material
Text:

### Exercise

## Uvicorn
COMING SOON

## Audio processing and Speech to Text Conversion
COMING SOON

# Capstone Project 
This capstone project is based on a real world open source project, which you can contribute to once you finish the capstone project

