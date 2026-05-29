# Request Body and Pydantic Fundamentals

## What is a Request Body?

A request body is the data sent by the client to the backend, usually in JSON format. It is commonly used with POST, PUT and PATCH requests.

Example:

{
"name": "Mani",
"email": "[mani@gmail.com](mailto:mani@gmail.com)"
}

Instead of sending large amounts of data through URLs, we send structured data in the request body.

## Why Do We Need Request Bodies?

* Cleaner APIs
* Easier validation
* Better scalability
* Industry standard approach

## What is Pydantic?

Pydantic is a data validation library used by FastAPI.

It validates incoming data automatically before it reaches the route function.

Example validations:

* Required fields exist
* Correct data types
* Invalid data is rejected

## Real World Understanding

Client sends JSON → FastAPI receives request → Pydantic validates data → Business logic executes → Response returned.

## IBM PlaySpace Booking Example

Possible fields:

* user_id
* game_id
* booking_date
* start_time
* participant_count

Server-generated fields:

* booking_id
* created_at
* updated_at
* booking_status

## Key Learning

The backend should only accept necessary input from the client. IDs and system-generated values should usually be created by the server.
