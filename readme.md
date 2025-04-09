# RestAPI for Creating QR Codes - Completed Assignment

## What Has Been Done

In this assignment, I successfully fixed several errors in the broken QR code API application. The project now passes all tests and is functioning correctly. Here's a summary of the completed steps:

1. ✅ **Cloned the broken repository** and set up the development environment
2. ✅ **Fixed multiple code issues**, including:
   - Fixed function name in `qr_service.py` (corrected `delete_qr_cde` to `delete_qr_code`)
   - Fixed route paths in `oauth.py` (corrected `/tokn` to `/token`)
   - Fixed route paths in `qr_code.py` (corrected `/qr-coes/` to `/qr-codes/`)
   - Fixed parameter names (`qr_fileame` to `qr_filename`)
   - Fixed field names in schema (`ul` to `url` and `mssage` to `message`)
   - Fixed admin password in config (`ecret` to `secret`)
   - Fixed typos in functions in `common.py`
   - Fixed router name in `main.py` (`ruter` to `router`)
3. ✅ **Created the QR codes directory** with proper permissions
4. ✅ **Ran tests locally to verify fixes** - all tests now pass!
5. ✅ **Set up Docker and tested the application** in a containerized environment
6. ✅ **Created a GitHub repository** at [https://github.com/Hameed1117/Broken_Qr_Code_Assignment](https://github.com/Hameed1117/Broken_Qr_Code_Assignment)
7. ✅ **Updated the GitHub Actions workflow file** to run tests and build Docker images
8. ✅ **Set up Docker Hub repository** at [https://hub.docker.com/repository/docker/khadhar17/qr_code_api](https://hub.docker.com/repository/docker/khadhar17/qr_code_api)
9. ✅ **Set up GitHub Secrets** for Docker Hub authentication

## How to Run the Application

1. Clone this repository
2. Create a virtual environment: `python3 -m venv venv`
3. Activate the virtual environment: `source venv/bin/activate`
4. Install requirements: `pip install -r requirements.txt`
5. Create QR codes directory: `mkdir -p qr_codes && chmod 777 qr_codes`
6. Run tests: `pytest`
7. Start the application: `docker-compose up --build`
8. Visit the API documentation at `http://localhost/docs`
9. Use the Swagger UI to test the API endpoints:
   - Authorize with username: `admin` and password: `secret`
   - Create, list, and delete QR codes

## CI/CD Pipeline

The application uses GitHub Actions for continuous integration and continuous deployment. The workflow:
1. Runs all tests to ensure code correctness
2. Builds a Docker image
3. Pushes the image to Docker Hub

The successful pipeline execution validates that all code issues have been fixed and the application is working as expected.