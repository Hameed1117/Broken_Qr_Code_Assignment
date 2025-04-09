RestAPI for Creating QR Codes - Completed Assignment
What Has Been Done
In this assignment, I successfully fixed several errors in the broken QR code API application. The project now passes all tests and is functioning correctly. Here's a summary of the completed steps:

✅ Cloned the broken repository and set up the development environment
✅ Fixed multiple code issues, including:

Fixed function name in qr_service.py (corrected delete_qr_cde to delete_qr_code)
Fixed route paths in oauth.py (corrected /tokn to /token)
Fixed route paths in qr_code.py (corrected /qr-coes/ to /qr-codes/)
Fixed parameter names (qr_fileame to qr_filename)
Fixed field names in schema (ul to url and mssage to message)
Fixed admin password in config (ecret to secret)
Fixed typos in functions in common.py
Fixed router name in main.py (ruter to router)


✅ Created the QR codes directory with proper permissions
✅ Ran tests locally to verify fixes - all tests now pass!
✅ Set up Docker and tested the application in a containerized environment
✅ Created a GitHub repository at https://github.com/Hameed1117/Broken_Qr_Code_Assignment
✅ Updated the GitHub Actions workflow file to run tests and build Docker images
✅ Set up Docker Hub repository at https://hub.docker.com/repository/docker/khadhar17/qr_code_api
✅ Set up GitHub Secrets for Docker Hub authentication

How to Run the Application

Clone this repository
Create a virtual environment: python3 -m venv venv
Activate the virtual environment: source venv/bin/activate
Install requirements: pip install -r requirements.txt
Create QR codes directory: mkdir -p qr_codes && chmod 777 qr_codes
Run tests: pytest
Start the application: docker-compose up --build
Visit the API documentation at http://localhost/docs
Use the Swagger UI to test the API endpoints:

Authorize with username: admin and password: secret
Create, list, and delete QR codes



CI/CD Pipeline
The application uses GitHub Actions for continuous integration and continuous deployment. The workflow:

Runs all tests to ensure code correctness
Builds a Docker image
Pushes the image to Docker Hub

The successful pipeline execution validates that all code issues have been fixed and the application is working as expected.