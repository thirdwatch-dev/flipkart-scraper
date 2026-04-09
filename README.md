# Flipkart Scraper

> Scrape Flipkart product listings, prices, ratings, and reviews -- India's largest e-commerce platform

[![Try on Apify](https://img.shields.io/badge/Try_on-Apify_Store-00C853?style=for-the-badge)](https://apify.com/thirdwatch)
[![Website](https://img.shields.io/badge/Website-thirdwatch.dev-000?style=for-the-badge)](https://thirdwatch.dev)

## What it does

Extracts product data from Flipkart, India's leading e-commerce marketplace. Collects product titles, prices, discounts, ratings, review counts, specifications, seller information, and delivery details. Ideal for Indian e-commerce market research and price tracking.

## Output fields

| Field | Type | Description |
|-------|------|-------------|
| title | String | Product title |
| price | Number | Current price in INR |
| originalPrice | Number | MRP before discount |
| discount | String | Discount percentage |
| rating | Number | Average rating (1-5) |
| reviewCount | Number | Total ratings and reviews |
| brand | String | Brand name |
| category | String | Product category |
| seller | String | Seller name |
| sellerRating | Number | Seller rating |
| images | Array | Product image URLs |
| specifications | Object | Product specs |
| url | String | Flipkart product URL |

## Input parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| queries | Array | Product search keywords |
| maxResults | Number | Maximum results per query |
| category | String | Category filter |
| sortBy | String | Relevance, price, rating, popularity |

## Example output

```json
{
  "title": "Samsung Galaxy S24 Ultra 5G (Titanium Gray, 256 GB)",
  "price": 129999,
  "originalPrice": 144999,
  "discount": "10% off",
  "rating": 4.5,
  "reviewCount": 28456,
  "brand": "Samsung",
  "category": "Mobiles",
  "seller": "SuperComNet",
  "sellerRating": 4.7,
  "images": ["https://rukminim2.flixcart.com/image/..."],
  "specifications": {
    "ram": "12 GB",
    "storage": "256 GB",
    "display": "6.8 inch Dynamic AMOLED"
  },
  "url": "https://www.flipkart.com/samsung-galaxy-s24-ultra/p/..."
}
```

## Pricing

| Plan | Price |
|------|-------|
| Pay per result | $0.002/result |
| Free tier | Available on Apify |

## Use cases

- India e-commerce price monitoring and tracking
- Competitive pricing analysis for Indian market
- Product catalog enrichment and data collection
- Indian consumer electronics market research
- Seller performance monitoring and benchmarking

## Getting started

1. Go to the [Apify Store](https://apify.com/thirdwatch)
2. Find the **Flipkart Scraper**
3. Enter product search keywords
4. Run and download results as JSON, CSV, or Excel

## Related scrapers by Thirdwatch

- [Amazon Scraper](https://github.com/thirdwatch-dev/amazon-scraper) -- Amazon products
- [IndiaMart Scraper](https://github.com/thirdwatch-dev/indiamart-scraper) -- B2B suppliers
- [JustDial Scraper](https://github.com/thirdwatch-dev/justdial-scraper) -- India business
- [Trustpilot Scraper](https://github.com/thirdwatch-dev/trustpilot-scraper) -- Reviews
- [Google Maps Scraper](https://github.com/thirdwatch-dev/google-maps-scraper) -- Business data

## About Thirdwatch

[Thirdwatch](https://thirdwatch.dev) builds production-ready web scraping APIs. 18 scrapers for jobs, e-commerce, reviews, social media, and business data.

## License

MIT
