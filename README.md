# Intel-Product Sentiment Analysis
### Project Members: Garv Bhaskar, Aviral Srivastava, Dinesh Kumar
### Institution: Vellore Institute of Technology, Chennai

## Installation and Setup

To run the files, you need to have `scrapy`, `glob`, and `BeautifulSoup` installed. Follow the steps below to set up and run the project.

### Prerequisites

Ensure you have Python installed. Then, install the required packages:

```bash
pip install scrapy beautifulsoup4
```

### Running the Scrapy Spider

1. Navigate to the `amazon` directory:
    ```bash
    cd amazon
    ```

2. Run the Scrapy spider:
    ```bash
    scrapy crawl amaze
    ```

### Output

The scraped data will be stored in `data.csv` located in the `amazon` directory.

## Notes

- Verify your internet connection as Scrapy needs to access the web for scraping.

For further customization or troubleshooting, refer to the Scrapy and BeautifulSoup documentation.
