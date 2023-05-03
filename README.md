# Neobis_Shortener_Project

URL Shortener is a Django-based web application that allows users to shorten long URLs into shorter, more manageable ones. This project uses Django Rest Framework (DRF) for building the API, and PostgreSQL for the database.
## Features

    - Shorten long URLs into shorter, more manageable ones
    - Generate unique short URLs using a custom algorithm
    - Store URLs and their shortened versions in a PostgreSQL database
    - Redirect users to the original URL when they visit the shortened version

## Installation

To install and run this project locally, follow these steps:

Clone the repository:

    $ git clone https://github.com/MIA1kl/Neobis_Shortener_Project.git

Navigate into the project directory:

    $ cd neo4UrlShort

Create and activate a virtual environment:

    $ python3 -m venv env
    $ source env/bin/activate

Install the project dependencies:

    $ pip install -r requirements.txt

Set up the database:

    $ python manage.py migrate

Start the development server:

    $ python manage.py runserver
    
***Access the application at http://localhost:8000/***

## API Endpoints

This project provides the following API endpoints:

    POST /api/create/: Create a new shortened URL
    GET /api/: List all shortened URLs
    GET /api/create/<id>/: Retrieve a specific shortened URL by ID
    GET /<shortcode>/: Redirect to the original URL associated with the given shortcode
    

### For more information on how to use these endpoints, please refer to the API documentation.

To view the API documentation, start the development server and navigate to http://localhost:8000/docs/.
Deployment

To deploy this project to a production environment, you will need to configure your own server and database. Some popular hosting options for Django applications include Heroku, AWS, and DigitalOcean.
Contributing
