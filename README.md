# DOCARE Backend

Welcome to the backend repository for **DOCARE PROJECT**! This repository contains the backend codebase implemented using Laravel 11 framework. The backend is structured as a set of microservices, each responsible for a specific domain of functionality.

## Microservices

### 1. Users Service
This microservice handles user-related functionalities such as user authentication, registration, profile management, etc.

### 2. Appointments Service
The Appointments Service manages all operations related to scheduling and managing appointments.

### 3. Records Service
The Records Service deals with functionalities related to storing and retrieving records or data.

## Getting Started
Follow the instructions below to set up and run the project locally:

### Prerequisites
- PHP >= 8.2
- Composer (Dependency Manager for PHP)

### Installation
1. Clone this repository to your local machine.
2. Navigate to the project directory:
    ```bash
    cd docare-backend
    ```
3. Navigate to the directory of the microservice you want to work with: 
    ```bash
    cd [name]-service
    ```
4. Install dependencies using Composer:
    ```bash
    composer install
    ```
5. Configure your environment variables by copying the `.env.example` file to `.env`:
    ```bash
    cp .env.example .env
    ```
6. Generate the application key:
    ```bash
    php artisan key:generate
    ```
7. Configure your database settings in the `.env` file.
8. Run database migrations to create necessary tables:
    ```bash
    php artisan migrate:fresh
    ```
9. Seed tables (Optional):
    ```bash
    php artisan db:seed
    ```

### Running the Application
To start the Laravel development server, run the following command:
```bash
php artisan serve
```
You can now access the microservice in your web browser.
You can repeat these steps for each microservice folder in your repository.

## Contributing Guidelines

To ensure a smooth workflow, contributors are kindly requested to adhere to the following guidelines:

1. **Microservice Specific Changes**: Make modifications only in the microservice assigned to you. Avoid making changes outside of your designated microservice to maintain clarity and prevent conflicts.

2. **Update from Develop**: Before submitting a pull request, ensure your local repository is up to date with the latest changes from the `develop` branch. This helps prevent merge conflicts and ensures your changes are based on the most recent codebase.

3. **Branching Strategy**: Create a new branch based on the `develop` branch for your changes. This keeps the main development branch clean and ensures that feature branches are easily identifiable.

4. **Pull Request Target**: Submit your pull requests targeting the `develop` branch. This allows for thorough review and testing of changes before they are merged into the main development branch.

5. **Review Process**: All pull requests will undergo a review process to ensure code quality, adherence to coding standards, and compatibility with the project's objectives.

6. **Main Branch Protection**: The `main` branch is read-only and protected against direct pushes. Changes to the main branch are only made through approved pull requests from the `develop` branch.

7. **Develop Branch Protection**: The `develop` branch is also protected against direct pushes. Every pull request targeting the `develop` branch will be reviewed before merging to maintain code integrity and project stability.

By following these guidelines, we can maintain a collaborative and organized development process. Thank you for your cooperation!

*Happy Coding Dev Team 😁👩‍💻👨‍💻*
Good luck
