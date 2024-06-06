# OnlineBookStore

Welcome to the OnlineBookStore, a web application built with Django that allows users to browse, search, and purchase books online.

## Features

- **User Authentication**: Sign up, log in, and manage your account.
- **Book Catalog**: Browse a wide variety of books.
- **Search Functionality**: Search for books by title, author, or genre.
- **Shopping Cart**: Add books to your cart and proceed to checkout.
- **Order Management**: View and manage your orders.
- **Admin Panel**: Admin interface to manage books, orders, and users.



## Installation

Follow these steps to get a local copy of the project up and running.

### Prerequisites

- Python 3.x
- Django 3.x or higher
- Virtualenv (optional but recommended)

### Setup

1. **Clone the repository**:

    ```bash
    git clone https://github.com/yourusername/OnlineBookStore.git
    cd OnlineBookStore
    ```

2. **Create and activate a virtual environment**:

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required packages**:

    ```bash
    pip install -r requirements.txt
    ```

4. **Apply the migrations**:

    ```bash
    python manage.py migrate
    ```

5. **Create a superuser** (to access the admin panel):

    ```bash
    python manage.py createsuperuser
    ```

6. **Run the development server**:

    ```bash
    python manage.py runserver
    ```

7. **Access the application**:

    Open your browser and navigate to `http://127.0.0.1:8000`

## Usage

- **Browse Books**: Explore the collection of books on the home page.
- **Search Books**: Use the search bar to find books by various criteria.
- **Add to Cart**: Click on a book and add it to your cart.
- **Checkout**: Proceed to checkout and place your order.
- **Admin Management**: Log in to the admin panel to manage books, users, and orders.

## Project Structure

```plaintext
OnlineBookStore/
│
├── bookstore/               # Main application folder
│   ├── settings.py          # Settings file for the project
│   ├── urls.py              # URL declarations for the project
│   ├── wsgi.py              # WSGI configuration
│   └── ...
├── books/                   # Books app
│   ├── models.py            # Database models
│   ├── views.py             # Views for handling requests
│   ├── urls.py              # URLs specific to books app
│   └── ...
├── cart/                    # Shopping cart app
│   ├── models.py            # Database models
│   ├── views.py             # Views for handling requests
│   ├── urls.py              # URLs specific to cart app
│   └── ...
├── orders/                  # Orders app
│   ├── models.py            # Database models
│   ├── views.py             # Views for handling requests
│   ├── urls.py              # URLs specific to orders app
│   └── ...
├── templates/               # HTML templates
│   ├── base.html            # Base template
│   └── ...
├── static/                  # Static files (CSS, JavaScript, images)
│   └── ...
├── manage.py                # Django's command-line utility
└── requirements.txt         # List of dependencies
