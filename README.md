# Loan Management API

This is a REST API for managing loans built with Lumen.
--

## Endpoints

- `POST /loans` - Create a new loan
- `GET /loans/{id}` - Get loan information by ID
- `PUT /loans/{id}` - Update loan information by ID
- `DELETE /loans/{id}` - Delete a loan by ID
- `GET /loans` - Get a list of all loans with basic filters by creation date and amount

## Setup

1. Clone the repository
    ```sh
    git clone <repository-url>
    ```

2. Navigate to the project directory
    ```sh
    cd lumen-api
    ```

3. Start the Docker containers
    ```sh
    docker-compose up -d
    ```

4. Run the composer install
    ```sh
    docker-compose run composer install
    ```

5. Run the migrations
    ```sh
    docker-compose run artisan migrate
    ```

6. Run the tests
    ```sh
    docker-compose exec php ./vendor/bin/phpunit tests/LoanTest.php
    ```
