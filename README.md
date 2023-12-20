# Flask Contacts API

This is a simple Flask-based API that manages contacts. It provides endpoints for CRUD operations on contacts stored in a SQLite database.

## Setup

1. Ensure you have Python installed on your system.
2. Install Flask and SQLAlchemy using pip:
pip install Flask SQLAlchemy
3. Clone this repository to your local machine.
4. Run the Flask application:
python app.py

5. The API will be available at `http://localhost:5000`.

## Endpoints

- `GET /contacts`: Retrieve all contacts.
- `POST /contacts`: Create a new contact.
- `GET /contacts/<id>`: Retrieve a specific contact by ID.
- `PUT /contacts/<id>` or `PATCH /contacts/<id>`: Update a specific contact by ID.
- `DELETE /contacts/<id>`: Delete a specific contact by ID.

## Database

This API uses a SQLite database named `contacts.db` to store contact information. The `Contact` model includes fields for `id`, `name`, `email`, and `phone`.

## Usage

You can interact with this API using HTTP requests. For example:

- To create a new contact:
POST /contacts
{
"name": "John Doe",
"email": "john@example.com",
"phone": "1234567890"
}

- To retrieve all contacts:
GET /contacts

- To update a contact with ID 1:

PUT /contacts/1
{
"name": "Jane Doe"
}

- To delete a contact with ID 2:
DELETE /contacts/2

Please make sure to handle responses appropriately and validate input data based on your application's requirements.
