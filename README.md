This is a simple dynamic web application built with Flask, styled using SimpleCSS, and extended with Redis for tracking visits and Pandas for data analysis of the Titanic dataset.
Features

    Homepage with a visit counter powered by Redis

    Navigation menu with links to:

        Home (visit tracker)

        Titanic (dataset viewer + chart)

        About (link to GitHub)

    Titanic dataset page showing:

        The first 5 rows of the dataset

        A bar chart of survivors by gender

    External link to HWR Berlin

    Static image served using Flask

    Responsive layout using SimpleCSS


How to Run Locally

    Clone the repo:

git clone https://github.com/juliusbgr/docker.git
cd docker

Create a virtual environment and install dependencies:

python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt

Set up a .env file (for Redis):

REDIS_HOST=localhost
REDIS_PASSWORD=yourpassword

Start Redis server (or use Docker if you prefer).

Run the Flask app:

    python app/app.py

Titanic Dataset

The app uses the Titanic dataset to demonstrate basic data handling with Pandas and visualization with Chart.js. Only Survived and Sex columns are required.

Created by juliusbgr