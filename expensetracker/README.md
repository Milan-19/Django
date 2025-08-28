# Django Expense Tracker

A simple and intuitive expense tracking application built with Django that helps you manage your income and expenses.

## Features

- Track income and expenses
- Real-time balance calculation
- Transaction history with delete functionality
- Clean and responsive user interface
- MySQL database integration

## Requirements

- Python 3.x
- Django 4.2.x
- MySQL

## Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd expensetracker
```

2. Create a virtual environment and activate it:

```bash
python -m venv env
source env/bin/activate  # On Windows use: env\Scripts\activate
```

3. Install dependencies:

```bash
pip install django mysqlclient
```

4. Configure MySQL database:

- Create a database named `expense_tracker`
- Update database settings in `expensetracker/settings.py` if needed

5. Apply migrations:

```bash
python manage.py migrate
```

6. Run the development server:

```bash
python manage.py runserver
```

7. Visit http://localhost:8000 in your browser

## Usage

- Add transactions using the form at the bottom of the page
- Enter positive numbers for income and negative numbers for expenses
- View your current balance, total income, and expenses
- Delete transactions using the trash icon

## Project Structure

```
expensetracker/
├── tracker/              # Main application
│   ├── models.py        # Database models
│   ├── views.py         # View logic
│   ├── urls.py         # URL routing
│   └── templates/      # HTML templates
├── public/              # Static files
│   └── static/
│       └── css/
├── expensetracker/      # Project settings
└── manage.py           # Django management script
```

## Contributing

Feel free to fork the project and submit pull requests for any improvements.

## License

This project is licensed under the MIT License.
