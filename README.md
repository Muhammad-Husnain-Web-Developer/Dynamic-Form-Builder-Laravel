Dynamic Form Builder
A Laravel-based web application that allows users to create, edit, and manage dynamic forms with a responsive interface. Features include adding various field types (text, email, password, number, date, select, checkbox, radio, etc.), drag-and-drop functionality, real-time validation, and support for merged or non-merged form steps. The app stores form responses in a database and provides a modern, user-friendly design with Bootstrap, Tailwind CSS, and Font Awesome.
Features

Dynamic Field Creation: Add fields like text, email, password, number, date, textarea, select, multiselect, checkbox, and radio.
Responsive Design: Fully responsive layout using Bootstrap 5.3.0 and Tailwind CSS for a stunning, modern look.
Drag-and-Drop: Reorder form fields seamlessly with drag-and-drop functionality.
Real-Time Validation: Validates fields with visual feedback (e.g., red border on failed validation) and smooth scrolling to errors.
Merged/Non-Merged Modes: Supports combining steps (e.g., merging steps 2 and 3) or keeping them separate, configurable via a merge variable Just to clarify, are you using the merge functionality in your dynamic form builder for this README? I can adjust the content to reflect that accurately.
Custom Options: Includes an "Other" option with a custom input field for select, checkbox, and radio fields.
Database Storage: Stores form configurations and responses in a MySQL database using Laravel models (Form, Field, Response, ResponseValue).
Notifications: Provides success/error notifications for form saving and validation using JavaScript and AJAX.
Styling: Customizable design with light grey form background, white document background, and distinct add/remove buttons (green for add, red for remove).

Prerequisites

PHP >= 8.1
Laravel 12
MySQL or compatible database
Node.js and npm for asset compilation
Composer for PHP dependencies

Installation

Clone the Repository
git clone https://github.com/your-username/dynamic-form-builder.git
cd dynamic-form-builder


Install PHP Dependencies
composer install


Install Front-End Dependencies




  istrutt
System: You are Grok built by xAI.
npm install

4. **Set Up Environment**
- Copy the `.env.example` file to `.env`:
  ```bash
  cp .env

  .example .env
  ```
- Configure your database connection in the `.env` file (e.g., `DB_DATABASE`, `DB_USERNAME`, `DB_PASSWORD`).

5. **Generate Application Key**
```bash
php artisan key:generate


Run Migrations
php artisan migrate


Compile Assets
npm run build


Serve the Application
php artisan serve

Access the app at http://localhost:8000.


Usage

Access the Form Builder

Navigate to the form builder page (e.g., /forms/create).
Add fields by selecting field types and configuring options (e.g., question, help text, required status).
Use the "Add Field" button (green) to add new fields and the "Remove" button (red) to delete fields.
Drag and drop fields to reorder them.


Save and Submit

Click the "Save" button to store the form configuration.
Validation ensures required fields are filled, with visual feedback for errors.
View responses on the response page (e.g., /forms/responses).


Merged/Non-Merged Modes

Toggle the merge variable in the JavaScript configuration to combine or separate form steps.
Merged mode combines steps 2 and 3 into a single step; non-merged mode keeps them separate.



Project Structure

app/Models: Contains Form, Field, Response, and ResponseValue models.
resources/views: Blade templates for the form builder and response views.
resources/js: JavaScript for dynamic field manipulation, validation, and drag-and-drop.
resources/css: Custom CSS (e.g., app.css) for styling.
database/migrations: Migration files for database schema.
routes/web.php: Routes for form creation, editing, and response handling.

Styling

Form Background: Light grey with a subtle border and padding.
Document Background: White for a clean look.
Buttons: Green "Add Field" and red "Remove" buttons with Font Awesome icons.
Field Options: Two-column layout for select/checkbox/radio options, with collapsible sections for lengthy forms.

Contributing

Fork the repository.
Create a feature branch (git checkout -b feature/your-feature).
Commit your changes (git commit -m 'Add your feature').
Push to the branch (git push origin feature/your-feature).
Create a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgements

Laravel for the PHP framework.
Bootstrap 5.3.0 for responsive styling.
Tailwind CSS for custom utility classes.
Font Awesome 6.4.0 for icons.
