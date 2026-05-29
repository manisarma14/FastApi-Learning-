# First Pydantic Model

BaseModel is the foundation of data validation in FastAPI.

A model acts as a schema that defines the expected structure of incoming data.

Example:

class UserCreate(BaseModel):
    name: str
    email: str
    password: str

Key Concepts:

- class creates a blueprint
- BaseModel provides validation
- name: str is a type hint
- Fields without default values are required
- Invalid or missing data results in automatic validation errors

Key Learning:

Pydantic models act as contracts between clients and the backend.