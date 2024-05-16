# Bestsellers Books Web Scraper

This Python script scrapes data from the Amazon Best Sellers Books section and exports it to a CSV file. The script retrieves information such as book names, authors, prices, ratings, and URLs for the best-selling books on Amazon.

## Dependencies

The script requires the following Python libraries:

- `requests`
- `beautifulsoup4`
- `csv`

You can install them using pip:

```
pip install requests beautifulsoup4
```

## Usage

1. Clone or download the repository to your local machine.
2. Navigate to the project directory.
3. Run either one of the scripts:

```
python com_bestseller.py
python in_bestseller.py
```

The script will scrape the data from the Amazon Best Sellers Books section and save it to a CSV file named `com_book.csv` in the `output` directory.

## Code Structure

The code follows these steps:

1. Retrieve the main page from the Amazon Best Sellers Books website.
2. Extract the links to all the pagination pages.
3. Iterate through each pagination page and extract the book details (name, author, URL, price, number of ratings, average rating).
4. Clean and format the extracted data.
5. Write the data to a CSV file with the following headers: `['Name', 'URL', 'Author', 'Price', 'Number of Ratings', 'Average Rating']`.

## Output

The script generates a CSV file named `com_book.csv` in the `output` directory. The file contains the following columns:

- `Name`: The book title.
- `URL`: The URL of the book on Amazon.
- `Author`: The author(s) of the book.
- `Price`: The price of the book.
- `Number of Ratings`: The number of ratings the book has received.
- `Average Rating`: The average rating of the book.

## Note

Please note that web scraping can be against the terms of service of some websites. Use this code responsibly and for educational purposes only.
