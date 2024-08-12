# Advance Blog Capstone Project

This project is an advanced blog platform built using Flask, SQLAlchemy, Flask-Bootstrap, Flask-CKEditor, and Flask-Login. It allows users to register, log in, create, edit, and delete blog posts, as well as comment on them. Only the admin has the ability to create, edit, and delete posts.

## Features

- **User Authentication:** Users can register, log in, and log out using Flask-Login.
- **Admin Panel:** Only the admin (user with ID 1) can create, edit, and delete posts.
- **Blog Posts:** Users can view all posts, and logged-in users can comment on them.
- **Comments:** Logged-in users can add comments to blog posts.
- **Gravatar Integration:** Users' profile images are displayed using Gravatar based on their email.
- **CKEditor:** A rich text editor for creating and editing blog posts and comments.

## Project Structure

- **main.py**: The main Flask application file that contains all routes and logic.
- **forms.py**: Contains the WTForms used for user registration, login, blog post creation, and commenting.
- **templates/**: Folder containing all HTML templates rendered by Flask.
- **static/**: Folder containing static files like CSS and JavaScript.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Prathamesh326/Advance-Blog-Capstone-Project.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Advance-Blog-Capstone-Project
   ```

3. Create and activate a virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   ```

4. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

5. Run the application:

   ```bash
   python main.py
   ```

   The application will start on `http://127.0.0.1:5002`.

## Usage

- Visit `http://127.0.0.1:5002/register` to create a new account.
- After registration, log in using the credentials you just created.
- Admin users can create, edit, and delete posts.
- All logged-in users can comment on posts.

## Database

- The database is configured to use SQLite, and it's stored in a file named `posts.db`.

## Admin Access

- To make a user an admin, manually update the user's ID to 1 in the database.
