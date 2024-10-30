# **To-Do List API**

This project is a RESTful API to manage a list of tasks using FastAPI and SQLite.

## **Requirements**
- Python 3.7 or higher
- pip (Python package manager)

## **Instalation**
1. Clone this repository:
   git clone <URL_DEL_REPOSITORIO>
   cd todo-api

2. Create and activate a virtual environment:
    python3 -m venv venv
    source venv/bin/activate

3. Install the dependencies:
    pip install fastapi uvicorn sqlalchemy

4. Run the server:
    uvicorn main:app --reload

## **Usage**

Open your browser and go to:  
[http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)  
This will open the Swagger UI where you can explore and test the API.

## **API Endpoints Overview**

- **GET /todos**: Retrieve a list of all tasks.
- **POST /todos**: Create a new task.  
  **Body:**  
  ```json
  {
    "title": "Task title",
    "description": "Optional description",
    "completed": false
  }
  ```
- **GET /todos/{todo_id}**: Retrieve a specific task by ID.
- **PUT /todos/{todo_id}**: Update a specific task by ID.  
  **Body:**  
  ```json
  {
    "title": "Updated title",
    "description": "Updated description",
    "completed": true
  }
  ```
- **DELETE /todos/{todo_id}**: Delete a specific task by ID.
