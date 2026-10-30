# Flipkart-Toys-Category-Sales-Pricing-Analysis-using-Power-BI
Project type: Business Intelligence | E-commerce Analytics |
Market Research
<p>Tools: Microsoft Power BI, Power Query, DAX
<p>Dataset: Web-scraped Flipkart toy product data

Project Overview
<p>This project explores a web-scraped dataset of toys listed on Flipkart.
The dashboard compares toy categories and sub-categories using product
availability, listed prices, customer reviews, and a review-based sales
proxy.

<p>The goal is to help sellers explore category-level patterns and identify
areas that may deserve further market research. The dataset does not
contain verified transaction, units-sold, revenue, cost, or profit data.
Business Questions
- Which toy categories contain the most listed products?
- Which categories receive the highest number of customer reviews?
- How do listed prices and review counts vary across categories?
- Which categories show a relatively high price-weighted review index?
- What areas could sellers investigate further before making inventory
  decisions?
Dashboard Preview
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/999e1b42-383e-4148-bd3e-f6d390961ccc" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/434b8fee-421d-4133-a21d-8d6220fadb93" />



Methodology
The analysis uses the following fields from the dataset:
- Product category and sub-category
- Product price
- Number of customer reviews
- Product listing / product count
Important metric definition
The original dashboard calculated:

Price × Number of Reviews

This value is not actual sales or revenue. It is a simple
price-weighted review proxy. It is affected by differences in review
behaviour, product age, and the time listings have been available.

For accurate reporting, this project should label the measure as:

Price-Weighted Review Index = Listed Price × Number of Reviews

It should not be described as sales, revenue, profit, or ROI.
Data limitation: Customer reviews are an imperfect indicator of
customer engagement and cannot be converted directly into units sold.
The index is useful only as a descriptive comparison within this
dataset.

Key Findings
1. Product availability
Based on the supplied analysis:
- Action Toys had the highest product count, with 352 products.
- Learning & Educational Toys followed with 321 products.
- LCD Writing Pads had 310 products.
2. Customer engagement
Based on total review counts:
- Baby Toys led with approximately 1.03 million reviews.
- LCD Writing Pads followed with approximately 513,000 reviews.
- Tricycles & Ride-ons had approximately 449,600 reviews.
These figures indicate review volume, not verified demand or units sold.
3. Price-weighted review index
The dashboard's original calculated measure showed:
- Tricycles & Ride-ons: approximately ₹1,003M index value.
- Baby Toys: approximately ₹284M index value.
- Soft Toys: approximately ₹130M index value.
These are outputs of the Price × Reviews calculation. They must not be
interpreted as actual sales or revenue.
Category Comparison
  Category            Product count      Sum of listed     Price-weighted
prices       review index
  Tricycles &                   100              ₹388K            ₹1,003M
Ride-ons                                             

  Baby Toys                     263              ₹121K              ₹284M
Soft Toys                     154               ₹75K              ₹130M
Values are reproduced from the supplied dashboard analysis and are
subject to the dataset's assumptions and limitations.
Business Interpretation
- Baby Toys lead in total customer reviews, making them a category
  worth exploring for customer-engagement patterns.
- Tricycles & Ride-ons have the highest price-weighted review
  index in this dataset. This is a signal for further investigation,
  not proof of profitability.
- Soft Toys also show a comparatively high index value and may
  warrant further category-level analysis.
- Product count should be considered alongside average price, average
  reviews per product, ratings, and competition before drawing
  investment conclusions.
Dashboard Features
- KPI cards for total index value, listed-price total, and product
  count
- Category filter
- Category-wise review distribution
- Comparison of listed prices and the price-weighted review index
- Category-level comparison table
- Sub-category comparison of the index and review counts
- Separate Cover, Dashboard, and Insights pages
Limitations and Assumptions
1. The dataset contains product-listing information, not verified sales
   transactions.
2. Review counts are used as a proxy for customer engagement; review
   rates vary between products.
3. Price × Reviews is a descriptive index, not actual sales, revenue,
   or profit.
4. The sum of listed product prices is not seller investment or
   procurement cost.
5. ROI cannot be calculated without reliable investment and
   return/profit data.
6. The analysis does not account for stock availability over time,
   discounts, shipping, platform fees, advertising, returns, or
   operating costs.
7. Results reflect the dataset snapshot and may not represent current
   Flipkart listings.
Recommended Further Analysis
To strengthen the analysis, the next version could include:
- Average listed price by category and sub-category
- Average reviews per product
- Median price and price-range distribution
- Average product rating, if available
- Products with high prices but low review counts
- Category-level competition indicators
- Data cleaning and missing-value documentation
- Clear DAX measure definitions and validation checks
A stronger investment recommendation would require actual sales volume,
seller costs, margins, inventory, and competition data.
Conclusion
The dashboard provides a category-level view of product availability,
review activity, and a price-weighted review index for Flipkart toy
listings. Baby Toys lead in total reviews, while Tricycles & Ride-ons
lead in the calculated index.

These findings can guide further market research, but they are not
sufficient on their own to establish actual sales performance or
profitability.

Repository Structure
Flipkart-Toy-Market-Analysis/
│
├── README.md
├── assets/
│   └── dashboard.png
└── powerbi/
    └── Flipkart_Toy_Sales_Dashboard.pbix
How to Use
1. Download or clone this repository.
2. Open the .pbix file in Microsoft Power BI Desktop.
3. If prompted, reconnect the dataset or update the source path.
4. Explore the dashboard pages and category filter.
Author: Shashwat Singh
Project focus: Power BI dashboarding, e-commerce data analysis, and
business intelligence
