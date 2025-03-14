# 🛒 Amazon Product Scraper

## 📌 Description
This Python script scrapes product details from Amazon using **requests** and **BeautifulSoup**. It extracts information like product title, price, rating, review count, and availability, then saves the data into a CSV file.

## 🌟 Features
- 📄 Scrapes multiple pages of Amazon search results
- 🔍 Extracts key product details:
  - 🏷️ Title
  - 💲 Price
  - ⭐ Rating
  - 🗣️ Number of reviews
  - 📦 Availability status
- 📊 Saves data into a structured CSV file

## ⚙️ Requirements
Make sure you have the following Python libraries installed:
```bash
pip install requests beautifulsoup4 pandas numpy
```

## 🚀 Usage
1. Update the `HEADERS` dictionary with a valid **User-Agent**.
2. Run the script:
   ```bash
   python amazon_scraper.py
   ```
3. The extracted data will be saved as `product_details.csv`.

## 📝 Code Overview
- **🆔 get_title(soup)**: Extracts product title.
- **💰 get_price(soup)**: Extracts product price.
- **⭐ get_rating(soup)**: Extracts customer rating.
- **🗣️ get_review_count(soup)**: Extracts number of reviews.
- **📦 get_availability(soup)**: Checks product availability.
- **🔄 Main script**:
  - Loops through multiple pages
  - Scrapes product links
  - Extracts details from individual product pages
  - Saves the data into a Pandas DataFrame and exports to CSV

## ⚠️ Notes
- **Amazon may block automated requests**. To avoid this:
  - Use rotating User-Agents and proxies.
  - Implement request delays.
- **Ensure compliance with Amazon's Terms of Service**.



