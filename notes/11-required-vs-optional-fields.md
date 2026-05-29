# Required vs Optional Fields

Required Fields:
Fields without default values.

Example:
name: str

Optional Fields:
Fields with default values.

Example:
age: int = 18

Optional fields can also use None as a default value.

Example:
phone: str | None = None

Key Learning:
Pydantic determines whether a field is required based on the presence of a default value.