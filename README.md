# FASTAPI
FastAPI boilerplate

## Setup

1. Create a virtual environment.
 ```sh
    python3 -m venv .venv
 ```
2. Activate virtual environment.
```sh
    source /path/to/venv/bin/activate`
```
3. Install project dependencies `pip install -r requirements.txt`
4. Create a .env file by copying the .env.sample file
`cp .env.sample .env`

5. Start server.
 ```sh
 python main.py
```


## Overview

This API provides endpoints for managing users, organisations, and related data for Your Project. It includes functionality for user management, organization management, social accounts, magic links, templates, pages, waitlist entries, charts, contents, and email templates.

### Database Schema Link
https://dbdiagram.io/d/Schema-Db-Main-669183769939893daecc89a2

### OpenAPI Specifications Link
https://app.swaggerhub.com/apis/FIFETOYI/devsWithSteeze/1.0.0#/

## Authentication

The API uses Bearer Token (JWT) for authentication.

Include the JWT token in the Authorization header for all requests.



This README provides an overview of the available API endpoints.

## Users
- `GET /users`: List users
- `POST /auth/register`: Register a user
- `POST /auth/login`: Login a user
- `GET /users/{userId}`: Get a user
- `PUT /users/{userId}`: Update a user
- `DELETE /users/{userId}`: Delete a user

## Organisations
- `GET /organisations`: List organisations
- `POST /organisations`: Create an organisation
- `GET /organisations/{organisationId}`: Get an organisation

## User Organisations
- `GET /user-organisations`: List user organizations
- `POST /user-organisations`: Add user to organization
- `GET /user-organisations/{id}`: Get a user organization
- `PUT /user-organisations/{id}`: Update a user organization
- `DELETE /user-organisations/{id}`: Delete a user organization

## Social Accounts
- `GET /social-accounts`: List social accounts
- `POST /social-accounts`: Add social account
- `GET /social-accounts/{id}`: Get a social account
- `PUT /social-accounts/{id}`: Update a social account
- `DELETE /social-accounts/{id}`: Delete a social account

## Magic Links
- `POST /magic-links`: Create magic link
- `GET /magic-links/{id}`: Get a magic link
- `DELETE /magic-links/{id}`: Delete a magic link

## Templates
- `GET /templates`: List templates
- `POST /templates`: Create template
- `GET /templates/{id}`: Get a template
- `PUT /templates/{id}`: Update a template
- `DELETE /templates/{id}`: Delete a template

## Pages
- `GET /pages`: List pages
- `POST /pages`: Create page
- `GET /pages/{id}`: Get a page
- `PUT /pages/{id}`: Update a page
- `DELETE /pages/{id}`: Delete a page

## Waitlist
- `GET /waitlist`: List waitlist entries
- `POST /waitlist`: Add to waitlist
- `GET /waitlist/{id}`: Get a waitlist entry
- `PUT /waitlist/{id}`: Update a waitlist entry
- `DELETE /waitlist/{id}`: Delete a waitlist entry

## Charts
- `GET /charts`: List charts
- `POST /charts`: Create chart
- `GET /charts/{id}`: Get a chart
- `PUT /charts/{id}`: Update a chart
- `DELETE /charts/{id}`: Delete a chart

## Contents
- `GET /contents`: List contents
- `POST /contents`: Create content
- `GET /contents/{id}`: Get a content
- `PUT /contents/{id}`: Update a content
- `DELETE /contents/{id}`: Delete a content

## Email Templates
- `GET /email-templates`: List email templates
- `POST /email-templates`: Create email template
- `GET /email-templates/{id}`: Get an email template
- `PUT /email-templates/{id}`: Update an email template
- `DELETE /email-templates/{id}`: Delete an email template

## Payments
- `POST /payments`: Create a payment
- `GET /payments`: Get all Payments
- `GET /payments/{id}`: Get a single payment information

## Blog Posts
- `GET /blog-posts`: List blog posts
- `POST /blog-posts`: Create a blog post

## Notifications
- `GET /notifications`: Get all notifications
- `POST /notifications`: Create a new notification
- `GET /notifications/{notificationId}`: Get a notification by ID
- `PUT /notifications/{notificationId}`: Update a notification by ID
- `DELETE /notifications/{notificationId}`: Delete a notification by ID


## Response Formats

All responses are returned in JSON format. Successful responses will have a 2xx status code, while errors will have appropriate 4xx or 5xx status codes.

## Error Handling

In case of errors, the API will return an appropriate HTTP status code along with a JSON object containing more details about the error.
