# T-Shirt E-Commerce Website

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Testing](#testing)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Overview
This project is a Laravel-based web application for managing an online T-shirt store. It provides a robust backend for handling products, categories, orders, and user management, along with a frontend for customers to browse and purchase T-shirts.

## Features
- **Product Management**: Add, edit, and delete T-shirt products with categories.
- **Category Management**: Organize products into categories for easier navigation.
- **Order Management**: Handle customer orders, including order creation, tracking, and status updates.
- **User Authentication**: Secure login and registration for customers and administrators.
- **Responsive Design**: A user-friendly interface optimized for both desktop and mobile devices.
- **Payment Integration**: (Optional) Integrate with payment gateways for seamless transactions.
- **Admin Dashboard**: Manage the store's inventory, orders, and users from a centralized dashboard.

## Project Structure
The project follows the standard Laravel directory structure:

```
laravel-project-t-shirt-website/
├── app/               # Core application logic (Models, Controllers)
├── bootstrap/         # Handles application bootstrapping
├── config/            # Configuration files
├── database/          # Migrations, Seeders, Factories
├── public/            # Public files (index.php, assets)
├── resources/         # Views, assets, language files
├── routes/            # Application routes (web.php, api.php)
├── storage/           # Logs, cached files, user uploads
├── tests/             # Unit and feature tests
```

## Prerequisites
Before running this project, ensure you have the following installed:
- PHP >= 8.0
- Composer
- Node.js and npm
- MySQL or another supported database

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/laravel-project-t-shirt-website.git
   cd laravel-project-t-shirt-website
   ```

2. Install PHP dependencies:
   ```sh
   composer install
   ```

3. Install JavaScript dependencies:
   ```sh
   npm install
   ```

4. Copy the environment configuration file:
   ```sh
   cp .env.example .env
   ```
   Then, configure your database and application settings in the `.env` file.

5. Generate the application key:
   ```sh
   php artisan key:generate
   ```

6. Run database migrations and seeders:
   ```sh
   php artisan migrate --seed
   ```

7. Build frontend assets:
   ```sh
   npm run dev
   ```

8. Start the development server:
   ```sh
   php artisan serve
   ```

## Testing
Run the test suite using PHPUnit:
```sh
php artisan test
```

## Deployment
For deployment, ensure you:
1. Set up a production database and configure the `.env` file.
2. Install optimized dependencies:
   ```sh
   composer install --optimize-autoloader --no-dev
   ```
3. Build production assets:
   ```sh
   npm run production
   ```
4. Set the correct permissions for the `storage` and `bootstrap/cache` directories.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

## License
This project is open-source and available under the MIT License.

## Acknowledgments
- Built with Laravel.
- Inspired by modern e-commerce platforms.

