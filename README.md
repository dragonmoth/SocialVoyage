# SocialVoyage

A social platform for travelers to connect and plan trips together.

## Prerequisites

- Python 3.8 or higher
- pip (Python package installer)
- MySQL/PostgreSQL database

## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/SocialVoyage.git
   cd SocialVoyage
   ```

2. **Create and Activate Virtual Environment**
   ```bash
   # Windows
   python -m venv venv
   venv\Scripts\activate

   # Linux/Mac
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Database Setup**
   ```bash
   # Create a database named 'socialvoyage'
   # Update database configuration in app.py with your credentials
   ```

5. **Environment Variables**
   Create a `.env` file in the root directory with the following:
   ```
   DATABASE_URL=your_database_url
   SECRET_KEY=your_secret_key
   ```

6. **Initialize Database**
   ```bash
   python init_db.py
   ```

7. **Run the Application**
   ```bash
   python app.py
   ```

8. **Access the Application**
   Open your browser and go to: `http://localhost:5000`

## Project Structure

```
SocialVoyage/
├── app.py
├── requirements.txt
├── .env
├── static/
│   ├── landing/
│   ├── login/
│   ├── profile/
│   ├── interests/
│   └── signup/
├── templates/
│   ├── index.html
│   ├── login.html
│   ├── profile.html
│   └── ...
└── README.md
```

## Common Issues and Solutions

1. **ModuleNotFoundError**
   - Solution: Make sure you've activated the virtual environment and installed all requirements

2. **Database Connection Error**
   - Solution: Check your database credentials in app.py
   - Ensure the database server is running
   - Verify the database exists

3. **Static Files Not Loading**
   - Solution: Check if all static files are present in the correct directories
   - Verify file permissions

4. **Port Already in Use**
   - Solution: Change the port in app.py or kill the process using the port

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
