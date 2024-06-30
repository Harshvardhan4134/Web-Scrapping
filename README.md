

# Amazon Web Scraper and Price Tracker

This Python script scrapes the title and price of a specific Amazon product and tracks changes over time. If the price drops below a certain threshold, it sends an email notification.

## Features

- Scrapes the Amazon product page for title and price information.
- Stores the scraped data (title, price, and date) in a CSV file (`AmazonWebScraperDataset.csv`).
- Checks the price daily and updates the CSV file.
- Sends an email notification if the price drops below $20 (adjustable threshold).

## Prerequisites

- Python 3.x
- Required Python libraries (`beautifulsoup4`, `requests`, `smtplib`, `datetime`, `time`, `csv`, `pandas`)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/amazon-web-scraper.git
   cd amazon-web-scraper
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Replace the `URL` variable in the script (`amazon_scraper.py`) with your desired Amazon product URL.
2. Update the `sender_email` and `password` variables in the `send_mail` function with your Gmail credentials.
3. Run the script:

   ```bash
   python amazon_scraper.py
   ```

4. The script will scrape the product page, update `AmazonWebScraperDataset.csv`, and send an email if the price drops below the specified threshold.

## Example CSV Format

| Title          | Price   | Date       |
| -------------- | ------- | ---------- |
| Product Title  | $XX.XX  | YYYY-MM-DD |

## Notes

- Ensure that you have configured your Gmail account to allow less secure apps to send emails if you're using Gmail for sending notifications.
- This script is intended for educational purposes. Use responsibly and respect Amazon's terms of service.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

### Additional Notes:
- **Structure**: Ensure your directory structure reflects the README. Place the script (`amazon_scraper.py`) and the CSV file (`AmazonWebScraperDataset.csv`) in the same directory.
- **Dependencies**: If you add any additional dependencies beyond what's listed, update `requirements.txt` and mention them in the installation instructions.

By following this template, users will have clear instructions on how to set up and use your Amazon web scraper and price tracker script. Adjust details like paths and specific instructions as necessary to fit your project’s setup.
