---
id: fastapi middleware
aliases:
  - middleware
tags:
  - fastapi
  - python
---

# Title: fastapi middleware

# Date: 09-02-2025

in fastapi we can use middleware to restrict calls from a particular domain.

```python
from fastapi import FastAPI
from fastapi.middleware.cors import CORSMiddleware

app = FastAPI()

origins = [
    "https://bull.mtnearth.com",
]

# Include localhost for development if needed
if os.getenv("ENVIRONMENT") == "development":
    origins.extend([
        "http://localhost:3000",
        "http://localhost:5173"  # If using Vite's default port
    ])

app.add_middleware(
    CORSMiddleware,
    allow_origins=origins,
    allow_credentials=True,
    allow_methods=["GET", "POST", "PUT", "DELETE", "OPTIONS"],
    allow_headers=["Authorization", "Content-Type"],
)
```
