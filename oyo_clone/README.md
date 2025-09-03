# OYO Clone - Hotel Booking Platform

A Django-based hotel booking platform inspired by OYO, featuring separate interfaces for users and hotel vendors.

## Features

### For Users

- User registration and authentication with email verification
- OTP-based login option
- Browse available hotels with filters
- Search hotels by name and location
- View hotel details, amenities, and images
- Book hotels with date selection
- Track booking history

### For Vendors

- Vendor registration with business details
- Email verification system
- Hotel management dashboard
- Add, edit, and manage hotel listings
- Upload and manage hotel images
- Track hotel bookings
- Manage amenities

## Tech Stack

- **Backend**: Django 4.2
- **Database**: MySQL
- **Frontend**: Bootstrap 5
- **Email**: SMTP (Gmail)
- **Image Storage**: Local Media Storage

## Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd oyo_clone
```

2. Create and activate virtual environment:

```bash
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Configure MySQL database:

- Create database named `oyo_clone_db`
- Update database settings in `settings.py`

5. Set up environment variables:

- Create `.env` file with:
  ```
  EMAIL_HOST_USER=your_email@gmail.com
  EMAIL_HOST_PASSWORD=your_app_password
  SECRET_KEY=your_secret_key
  ```

6. Run migrations:

```bash
python manage.py migrate
```

7. Start development server:

```bash
python manage.py runserver
```

## Project Structure

```
oyo_clone/
├── accounts/          # User and vendor authentication
├── home/              # Main hotel listing and booking
├── media/            # Uploaded files
│   ├── amenities/    # Amenity icons
│   └── hotels/       # Hotel images
├── static/           # Static files
└── templates/        # HTML templates
```

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License.

## Acknowledgments

- OYO for inspiration
- Django community
- Bootstrap team
