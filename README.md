Dynamic Form Builder

A powerful Laravel-based web application for creating and managing dynamic forms. Build responsive forms with drag-and-drop functionality, real-time validation, and customizable field types (text, email, select, checkbox, etc.). Supports merged or non-merged form steps and stores responses in a MySQL database.
Features

Dynamic Fields: Add text, email, password, number, date, textarea, select, multiselect, checkbox, and radio fields.
Drag-and-Drop: Reorder fields effortlessly with a user-friendly interface.
Real-Time Validation: Instant feedback with red borders for errors and smooth scrolling to invalid fields.
Merged/Non-Merged Modes: Combine steps (e.g., steps 2 and 3) or keep them separate via a merge configuration.
Responsive Design: Built with Bootstrap 5.3.0 and Tailwind CSS for a modern, mobile-friendly UI.
Custom Options: Includes "Other" input for select, checkbox, and radio fields.
Database Storage: Saves form configurations and responses using Laravel models (Form, Field, Response, ResponseValue).
Notifications: Success/error alerts for form actions via JavaScript and AJAX.
Styling: Light grey form background, white document background, green "Add" and red "Remove" buttons with Font Awesome icons.

Prerequisites

PHP >= 8.1
Laravel 12
MySQL or compatible database
Node.js and npm
Composer

Installation

Clone the Repository
git clone https://github.com/your-username/dynamic-form-builder.git
cd dynamic-form-builder


Install Dependencies
composer install
npm install


Configure Environment

Copy .env.example to .env:cp .env.example .env


Update .env with your database credentials (e.g., DB_DATABASE, DB_USERNAME, DB_PASSWORD).


Generate Application Key
php artisan key:generate


Run Migrations
php artisan migrate


Compile Assets
npm run build


Start the Server
php artisan serve

Access at http://localhost:8000.


Usage

Create a Form

Go to /forms/create.
Add fields, configure options (e.g., question, required status), and reorder via drag-and-drop.
Use green "Add Field" and red "Remove" buttons.


Submit and Validate

Save forms with validation checks.
View responses at /forms/responses.


Toggle Modes

Set merge in JavaScript config to combine or separate form steps.



Project Structure

app/Models: Laravel models for forms and responses.
resources/views: Blade templates for UI.
resources/js: JavaScript for dynamic features.
resources/css: Custom styles (app.css).
database/migrations: Database schema.
routes/web.php: Application routes.

Contributing

Fork the repository.
Create a branch: git checkout -b feature/your-feature.
Commit changes: git commit -m 'Add your feature'.
Push: git push origin feature/your-feature.
Submit a pull request.

License
MIT License
Acknowledgements

Laravel
Bootstrap 5.3.0
Tailwind CSS
Font Awesome 6.4.0
