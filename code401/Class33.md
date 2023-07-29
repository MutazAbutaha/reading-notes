# Read: Class 33

## What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?

JSON Web Tokens (JWTs) serve as a secure method for authentication and authorization in web applications. They work by encoding user data and a signature into a compact string, which can be transmitted between parties. The server generates a JWT upon user login, and subsequent requests from the client include the token. The server then decodes the JWT to verify the user's identity and permissions.

## How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?

JWT Authentication in Django REST Framework enables secure API endpoints by validating user identity through JWT tokens. The process involves sending the token in the request headers upon user login. Django REST Framework's authentication classes verify the token's validity, and if successful, grant access to the protected API endpoints. Key components include DRF's authentication classes, token generation upon login, and token validation during subsequent requests.

## Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?

Django's built-in runserver is not suitable for production environments due to its limited capabilities and potential security vulnerabilities. It is single-threaded, lacks performance optimizations, and may not handle high traffic well. For production deployment, alternatives like Gunicorn, uWSGI, or ASGI servers like Daphne are recommended. These options provide better performance, concurrency, and scalability to ensure a stable and secure environment for Django applications.
