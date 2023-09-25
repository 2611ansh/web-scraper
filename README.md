# Web Scraping and Review Analysis with Flask

This is a Python web application that scrapes product reviews from Flipkart and stores them in a MongoDB database. It uses the Flask web framework for creating a web interface to input search queries and display the results.

## Features

- Scrapes product reviews from Flipkart based on user input.
- Stores the scraped data in a MongoDB database.
- Provides a web interface to input search queries and view the results.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.x installed on your system.
- Required Python libraries: Flask, Flask-CORS, requests, BeautifulSoup (bs4), pymongo.

## Setup and Usage

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/flipkart-review-scraper.git
   ```

2. Navigate to the project directory:

   ```bash
   cd flipkart-review-scraper
   ```

3. Install the required Python libraries using pip:

   ```bash
   pip install Flask Flask-CORS requests BeautifulSoup4 pymongo
   ```

4. Run the application:

   ```bash
   python app.py
   ```

   The application will start and be accessible at `http://127.0.0.1:8000/` in your web browser.

5. Use the web interface to input search queries and retrieve product reviews from Flipkart.

## Code Structure

- `app.py`: The main Flask application file.
- `templates/`: Contains HTML templates for the web interface.
- `static/`: Contains static files (e.g., CSS, JavaScript) for the web interface.

## Configuration

You need to configure the MongoDB connection in the `app.py` file. Update the following line with your MongoDB connection string:

```python
client = pymongo.MongoClient("mongodb+srv://username:password@cluster.mongodb.net/?retryWrites=true&w=majority")
```

Replace `username`, `password`, and `cluster.mongodb.net` with your MongoDB credentials.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This project uses Flask, a micro web framework for Python.
- BeautifulSoup is used for parsing HTML content.
- MongoDB is used as the database for storing scraped data.

---

Feel free to customize this README as needed and add any additional information or instructions.
