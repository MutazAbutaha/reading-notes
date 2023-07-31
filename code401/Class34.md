# Read: Class 34

## What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?

### Django Settings Best Practices:

* Organize settings into separate files for different environments.
* Avoid hardcoding sensitive information; use environment variables.
* Use default settings where possible and maintain consistency in naming.
* Keep settings files in version control but exclude sensitive data.

## How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project?

### White Noise and Serving Static Files in Django:

* White Noise efficiently serves static files in production.
* It acts as WSGI middleware and reduces load on Python process.
* Install it using pip, add middleware to settings, and configure storage.
* Ensure your web server is set up correctly to use White Noise.

## What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?

### Cross-Origin Resource Sharing (CORS) in Django:

* CORS prevents unauthorized requests to different domains.
* Use django-cors-headers for handling CORS in Django.
* Install the package, add middleware to settings, and configure origins.
* Django includes appropriate CORS headers in responses based on configuration.
