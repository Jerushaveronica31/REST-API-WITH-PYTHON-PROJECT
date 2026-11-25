# REST-API-WITH-PYTHON-PROJECT
# REST APIs with Python (`requests` & `FastAPI`)

A hands-on notebook (`JERUSHA_VERONICA_API.ipynb`, exported as `jerusha_veronica_api.py`) demonstrating how to consume public REST APIs with `requests` and build a CRUD API using `FastAPI` and `Pydantic`.

## Overview

This project covers client-side HTTP operations, JSON parsing, request headers and error handling, and server-side API creation with endpoint testing using FastAPI's `TestClient`.

## What's Covered

- **Consuming REST APIs (`requests`)**
  - Inspecting HTTP status codes, response headers (`Content-Type`), and JSON payloads[cite: 2]
  - Filtering results with query parameters (`params`)[cite: 2]
  - Performing `GET`, `POST`, `PUT`, `PATCH`, and `DELETE` requests[cite: 2]
  - Working with JSON strings and Python dictionaries via `json.dumps()` and `json.loads()`[cite: 2]
  - Passing custom headers (`Accept` and `Authorization: Bearer ...`)[cite: 2]
  - Handling request timeouts (`timeout=10`), `raise_for_status()`, and `requests.exceptions`[cite: 2]
- **Building a REST API (`FastAPI` + `Pydantic`)**
  - Defining basic routes (`/` and path parameter route `/hello/{name}`)[cite: 2]
  - Validating request bodies with a `Student` `BaseModel` schema (`name: str`, `age: int`, `course: str`)[cite: 2]
  - Implementing full CRUD endpoints for `/students` (`GET /students`, `GET /students/{student_id}`, `POST /students`, `PUT /students/{student_id}`, `DELETE /students/{student_id}`)[cite: 2]
  - Returning `404` errors with `HTTPException` when a student record is not found[cite: 2]
  - Testing endpoints in-memory using `fastapi.testclient.TestClient`[cite: 2]

## Tech Stack

- **Python**[cite: 2]
- **requests**[cite: 2]
- **FastAPI**[cite: 2]
- **Pydantic**[cite: 2]
- **httpx**[cite: 2]
- **Google Colab**[cite: 2]

## How to Run

1. Install dependencies:
   ```bash
   pip install requests fastapi httpx
