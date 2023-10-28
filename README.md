# DevOps-Capstone-1
# Abode Software DevOps Lifecycle Implementation

## Project Overview
This project aims to implement the DevOps lifecycle for Abode Software's product available at [Abode Software GitHub Repository](https://github.com/hshar/website.git). The goal is to set up a streamlined DevOps process to automate software deployment and testing.

## Implementation Steps

### 1. Installation of Necessary Software
- Utilize the chosen configuration management tool to install required software on machines. This ensures consistency and reduces manual setup efforts.

### 2. Git Workflow Setup
- Implement Git workflow for version control. Ensure that the master and develop branches are appropriately managed, following the branching strategy.

### 3. CodeBuild Integration
- Configure CodeBuild to automate builds triggered by commits to the master or develop branches:
    - If a commit is made to the master branch, execute tests and push to production.
    - If a commit is made to the develop branch, solely test the product without pushing to production.

### 4. Docker Containerization
- Implement containerization of the code using a Dockerfile. Ensure the Dockerfile is built on every push to the GitHub repository.
    - Utilize the pre-built container 'hshar/webapp' for the application.
    - The code should reside in the '/var/www/html' directory within the container.

### 5. Jenkins Pipeline Setup
- Define the tasks in a Jenkins Pipeline, configuring the following jobs:
    - Job1: build
    - Job2: test
    - Job3: prod

## Steps for Execution
Follow the steps below to execute the DevOps lifecycle implementation:

### Prerequisites
- Access to the Abode Software GitHub repository.
- Permissions to configure the chosen configuration management tool, Git, Docker, AWS CodeBuild, and Jenkins.

### Execution Steps
1. Clone the Abode Software GitHub repository:
    ```bash
    git clone https://github.com/hshar/website.git
    ```
2. Set up and configure the chosen configuration management tool for software installation on the machines.
3. Implement the Git workflow as per the branching strategy mentioned.
4. Configure and integrate AWS CodeBuild according to the specified conditions for master and develop branches.
5. Create a Dockerfile in the root of the project to containerize the application.
6. Set up Jenkins and define a Pipeline with the designated jobs: build, test, and prod.

## Additional Notes
- Ensure proper testing and validation of each stage in the pipeline before proceeding to the next stage.
- Regularly monitor and ensure the pipeline's efficiency and stability.

For detailed step-by-step implementation, refer to the project's documentation or reach out to the DevOps team.

For any queries or support, contact: [Your Contact Information]
