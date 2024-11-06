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
1. Database and CRUD Operations
2. ORM (including orm vs raw sql)
3. 
### Learning Material

### Exercise


## Websockets
### Concepts

### Learning Material

### Exercise



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

