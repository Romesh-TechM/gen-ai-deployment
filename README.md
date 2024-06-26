﻿# gen-ai-deployment

name: The name of the workflow.
on: Defines when the workflow should be triggered. In this case, it runs on pushes to the main branch and pull requests targeting the main branch.
jobs: Contains one or more jobs to be executed.
build: Name of the job.
runs-on: Specifies the type of runner for the job, in this case, Ubuntu.
steps: Contains a sequence of tasks to be executed.
Checkout code: Checks out the repository code.
Set up Python: Sets up the Python environment.
Install dependencies: Installs required dependencies like flake8, black, bandit, and pytest.
Lint code: Runs flake8 for linting the code.
Format code: Runs black to format the code.
Security check: Runs bandit to check for security issues.
Run tests: Executes Pytest to run the tests.
