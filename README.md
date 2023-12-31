# REST-API with MongoDB and FastAPI

This is a simple REST-API that supports CRUD operations. It is built using FastAPI and PyMongo.
PyMongo is the official MongoDB driver for Python. It also helps if you have MongoDB Compass installed on your machine.

## Setup

Create an `.env` file and add the following variables:

```
ATLAS_URI = "****"
DB_NAME = "****"
```

Run the followng command in the terminal to install the dependencies:
(Make sure you are at the root directory of the project)

```bash
python -m pip install 'fastapi[all]' 'pymongo[srv]' python-dotenv
```

If you intend to run tests, you need to install `pytest`:

```bash
python -m pip install pytest
```

Then run this command:

```bash
python -m pytest
```

## Testing the endpoints

Run this command in the terminal:

```bash
python -m uvicorn main:app --reload
```

Navigate to  http://localhost:8000/docs in your browser. FastAPI and Swagger provide a UI that we can use to test the various endpoints.