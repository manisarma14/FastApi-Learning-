# Pydantic BaseModel

## What is BaseModel?

BaseModel is the foundation of data validation in FastAPI.

## Why Use It?

- Defines request schema
- Validates incoming data
- Converts JSON into Python objects
- Reduces manual validation code

## Key Concepts

Schema:
Defines expected structure of data.

Field:
Individual attribute in a model.

Validation:
Ensures data follows required rules.

## Request Flow

Client Request
→ Pydantic Model
→ Validation
→ Route Function
→ Response

## Key Learning

BaseModel acts as a contract between client and server and ensures only valid data reaches business logic.