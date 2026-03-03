<h1 align="center">🚨 EMSUGI 🚨</h1>

  


## Table of Contents
- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Screenshots](#screenshots)
- [Getting Started](#getting-started)
  - [Tech Stack](#tech-stack)
  - [Installation](#installation)
  - [Running with Docker](#running-with-docker)
  - [Folder Structure](#folder-structure)
- [Usage](#usage)
- [Contributing](#contributing)
- [MIT License](#mit-license)

## Project Overview

The **EMSUGI** is a sophisticated application designed to gather and analyze emergency alerts from various sources. It leverages generative AI to predict future incidents based on historical data and current trends. This system aims to enhance the efficiency of emergency responses by providing insightful reports and visual analytics.


## Key Features:
- **Real-Time Alert Monitoring**: Fetches and stores emergency alerts across different countries.
- **Generative AI**: Implements AI to analyze and generate future predictions of emergency incidents.
- **Graphical Representation**: Displays data using charts and graphs, allowing users to visualize key metrics.
- **Interactive Date/Time Range Selection**: Enables users to set custom date and time ranges for report generation.
- **Keyword and Topic Analysis**: Identifies popular keywords and topics by country and region.
- **Responsive Design**: Supports a mobile-friendly and responsive layout for viewing reports.


> **NOTE:** These features are based project's future intention so the actual performance and feature may vary due to active development phases

## Screenshots

Below are some screenshots showing the features and layout of the system:

<img src="https://github.com/user-attachments/assets/41b35a5b-043c-47db-b19c-9ae92a423356" width="200">
<img src="https://github.com/user-attachments/assets/78edc4fa-53a8-4427-9cdb-8b58bd9ecbb5" width="200">
<img src="https://github.com/user-attachments/assets/38c8673f-d62b-4ddd-b1a0-9ff19068603a" width="200">
<img src="https://github.com/user-attachments/assets/e64d8b90-4d55-425c-b69d-3ad38bce5d5c" width="200">
<img src="https://github.com/user-attachments/assets/b8c5bed8-d13d-4384-b20d-a9de6d3bba94" width="200">
<img src="https://github.com/user-attachments/assets/658f0d48-ca7b-457c-96af-1b608db89c2e" width="200">
<img src="https://github.com/user-attachments/assets/1381e445-8603-48c4-b7e1-9276fa89965d" width="200">
<img src="https://github.com/user-attachments/assets/6b17ecbd-3603-45dc-8340-b1c7d8c0b45f" width="200">

> **NOTE:** These screenshots reflect the current state of the project's development and may change in the future as features evolve and improvements are made.

## Getting Started

### Tech Stack:

- **Python** (Version 3.x or higher): A powerful, high-level programming language used for backend development.  
- **Flask**: A lightweight web framework for building web applications in Python.  
- **pandas**: A data manipulation library that provides powerful data structures for data analysis.  
- **matplotlib**: A popular plotting library used for creating static, animated, and interactive visualizations.  
- **gemini**: An AI-powered tool for generative report generation, used for creating emergency and disaster reports.  
- **torch**: A deep learning framework that provides flexible and efficient tools for training and deploying machine learning models, particularly for local model inference.  
- **transformers**: A library by Hugging Face for working with pre-trained transformers and other state-of-the-art machine learning models.  
- **logly**: A logging and monitoring tool used to track and manage logs within applications.  
- **python-dotenv**: A tool to manage environment variables, allowing the configuration of sensitive information (API keys, tokens, etc.) in a `.env` file.  
- **SQLite**: A lightweight, disk-based database to store and retrieve data for the application.  
- **Tailwind CSS**: A utility-first CSS framework for quickly designing responsive, modern web interfaces.
- **Font Awesome** - Icon library used for adding scalable vector icons in the UI.
- **Chart.js** - JavaScript library for creating interactive and customizable charts for data visualization.

### Installation:

1. Clone the repository:
   ```bash
   git clone https://github.com/Vishnu-KumarKR/Emergency-Managment-System-Using-GenAI.git
   cd EMSUGI
   ```

2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```


3. Run the Flask Web UI:
   ```bash
   python launch.py
   ```

4. Open your browser and go to:
   ```
   http://127.0.0.1:5000/
   ```
### Running with Docker

If you'd like to run this project using Docker, check out the [docker_readme.md](DOCKER_README.md) file for a step-by-step guide on building, 
running, and managing the EMSUGI application in a Docker container.

### Folder Structure:
```bash
.
├── launch.py                  # Launch Flask application
├── modules/                # Application modules
│   ├── api/                # API endpoints
│   │   ├── __init__.py    # Initialize API endpoints
│   │   ├── loading.py      # Loading API endpoint
│   │   ├── cancel_process.py      # Cancel the report generation process
│   │   .
│   │   .
│   ├── fetch_alerts.py     # Fetch report from online
│   ├── generate.py  # Generate report
│   ├── process.py  # Process the report
│   ├── router.py  # Router for the application
│   ├── db.py # Database connection
│   ├── download.py # Download the models
│   ├── async_worker.py # Async worker for the application
│   ├── routes/            # Application routes
│   │   ├── __init__.py    # Initialize application routes
│   │   ├── index_page.py      # Index Page route
│   │   ├── report_page.py      # Report Page route
│   │   ├── analytics_page.py      # Analytics Page route
│   │   ├── notice_page.py      # Notice Page route
│   │   ├── license_page.py      # License Page route
│   │   ├── records_page.py      # Records Page route
│   │   ├── reports_page.py      # Reports Page route
│   ├── utils/              # Utility functions
│   │   ├── __init__.py    # Initialize utility functions
│   │   └── progress.py     # Progress utility functions
│   │   └── check_for_cancel.py # Check if the report generation has been canceled
│   │   .
│   │   .
├── templates/              # Contains HTML templates
│   └── index.html          # Main HTML file
├── static/                 # Static files (CSS, JS, images)
│   ├── styles.css          # Global styles
├── create_database.py      # Used to create DB
├─��� database_alerts.db      # Stored Database
├── Dockerfile              # Docker configuration file
├── CODE_OF_CONDUCT.md      # Code of conduct for contributors
├── LICENSE                 # Open-source license for the project
├── pyproject.toml          # Python project configuration file
├── docker_readme.md        # Instructions for using Docker
└── README.md               # Project documentation
```

## Usage

- Open the application in your browser.
- Enter a range of dates and times to generate reports.
- Visualize the results in various graphical formats.





