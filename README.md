# 🚀 Dynamic Form Builder

A feature-rich, **Laravel-based** web application for creating and managing dynamic forms with a sleek, responsive interface. Build forms effortlessly with **drag-and-drop**, **real-time validation**, and support for various field types (text, email, select, checkbox, etc.). Choose between **merged or non-merged form steps** and store responses in a **MySQL database**. Styled with **Bootstrap**, **Tailwind CSS**, and **Font Awesome** for a modern look.

---

## ✨ Features

| Feature              | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| **Dynamic Fields**   | Create fields like text, email, password, number, date, textarea, select, multiselect, checkbox, and radio. |
| **Drag-and-Drop**    | Reorder fields intuitively with a smooth drag-and-drop interface.            |
| **Real-Time Validation** | Instant feedback with red borders for errors and auto-scroll to invalid fields. |
| **Merged/Non-Merged Modes** | Combine steps (e.g., steps 2 and 3) or keep separate using a merge config. |
| **Responsive Design** | Mobile-friendly UI with **Bootstrap 5.3.0** and **Tailwind CSS**.           |
| **Custom Options**   | Add an "Other" input for select, checkbox, and radio fields.                 |
| **Database Storage** | Store form configurations and responses using Laravel models.                |
| **Notifications**    | Success/error alerts via JavaScript and AJAX.                                |
| **Styling**          | Light grey form background, white document background, modern buttons & icons. |

---

## 🛠️ Prerequisites

Before you begin, ensure you have the following installed:

- **PHP >= 8.1**
- **Laravel 12**
- **MySQL** or compatible database
- **Node.js** and **npm** (for asset compilation)
- **Composer** (for PHP dependencies)

---

## 📦 Installation

Follow these steps to set up the project locally:

```bash
# Clone the Repository
git clone https://github.com/Muhammad-Husnain-Web-Developer/Dynamic-Form-Builder-Laravel.git
cd dynamic-form-builder

# Install Dependencies
composer install
npm install

# Configure Environment
cp .env.example .env
