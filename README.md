# Module 8

Dockerhub URL:
https://hub.docker.com/r/desroca/601_module8

## Objective
For this assignment, I enhanced and tested a FastAPI-based calculator application by writing unit, integration, and end-to-end tests. I also implemented logging and configured GitHub Actions for continuous integration (CI).

The goal was to verify that the calculator's arithmetic operations work correctly, that the API endpoints respond as expected, and that the application can be tested automatically through a CI workflow.

## Assignment Requirements

The assignment required the following:

1. Set up the FastAPI calculator application and install its dependencies.
2. Write unit tests for all functions in `operations.py`.
3. Write integration tests for the API endpoints in `main.py`.
4. Implement end-to-end tests using Playwright to simulate user interactions.
5. Implement logging to track calculations and errors.
6. Use Git for version control and commit changes regularly.
7. Configure GitHub Actions to run tests automatically when changes are pushed.
8. Submit the GitHub repository link and screenshots showing a successful GitHub Actions workflow and the application running in a browser.

## Implementation

- Added unit tests for the functions in `app/operations/__init__.py`.
- Added integration tests for the API endpoints in `main.py`.
- Added end-to-end tests using Playwright.
- Implemented logging to record successful calculations and errors.
- Configured logging through environment variables using `python-dotenv`.
- Updated `.gitignore` to exclude environment configuration files and generated logs.
- Configured GitHub Actions to run tests automatically when changes are pushed.

## Instructions

1. Clone the repository.
2. Create and activate a virtual environment.
3. Install the required dependencies:
   pip install -r requirements.txt
4. Create a `.env` file in the project root and add:
   `CALCULATOR_LOG_FILE=logs/calculator.log`
5. Run the application:
   `docker-compose up --build`
6. open `localhost:8000` in your browser.
7. Run tests:
   'pytest'