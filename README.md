# BestLego

The project analyzes customer reviews of LEGO products on Amazon to uncover consumer preferences, trends, and insights that can guide businesses, marketers, and LEGO enthusiasts in understanding popular products and their performance.

## Purpose of Analysis

- **Guide LEGO Fans**: Help fans identify the most popular and loved LEGO sets within the budget range of $50 to $150.
- **Provide Insights to Business Owners**: Deliver valuable insights into customer sentiment and product performance to improve product offerings.
- **Support Marketers**: Enable marketers to refine campaigns based on sentiment analysis and review trends.
- **Empower Strategic Decision-Making**: Provide actionable insights for stakeholders in the LEGO marketplace.

## Business Questions

- **Distribution of Overall Rating**: What is the overall rating distribution for LEGO products?
- **Highest Review Dates**: When are the peak periods for reviews?
- **Common Review Themes**: What are the recurring themes in customer reviews?
- **Top-Rated LEGO Products**: Which LEGO products receive the highest ratings?
- **Average Ratings Over Time**: How do average ratings vary over different periods?
- **Most Active Reviewers**: Who are the most active reviewers?
- **Proportion of Positive/Negative Reviews**: What is the balance of positive vs. negative reviews?

## Web Scraping from Amazon.com

- **Methodology**: Used web scraping techniques to gather customer reviews for LEGO products from Amazon to build the dataset.
- **Data Characteristics**: Reviews were collected for a wide range of LEGO products, focusing on sentiment, rating distribution, and thematic trends.

## Key Findings

### Distribution of Overall Ratings
- Most reviews are rated highly, indicating customer satisfaction with LEGO products.

### Common Themes in Reviews
- LEGO products are primarily associated with gifts for boys, with common keywords like "cars," "bikes," "sons," "grandsons," "fun," "great," and "good."
- Themes highlight building experiences and product quality/value.

### Dates with Highest Reviews
- Peak review dates include **2005-10-19** and **2008-06-08**, with up to 35 reviews per day, likely influenced by Amazon’s review limits.

### Top-Rated LEGO Products
- Some of the highest-rated LEGO products include:
  - **LEGO Jurassic Triceratops Velociraptor** (5.0 Rating)
  - **LEGO Magic Maze** (5.0 Rating)
  - **LEGO Kristoff’s Sleigh Adventure** (5.0 Rating)

### Average Ratings Across Periods
- **2005**: Had the lowest average ratings, possibly due to limited internet access and fewer reviews.
- **2024 Q3**: Saw a significant drop in ratings, primarily due to an anomaly in July 2024.

### Most Active Reviewers
- Active reviewers like "Amazon Customer" reviewed up to 490 products, though many users prefer to remain anonymous.

### Proportion of Positive/Negative Reviews
- **Very Positive Reviews**: 76.92%
- **Very Negative Reviews**: 1.92%

## NLP & Gensim Topic Modeling Analysis

### Common Themes in Reviews (NLP)
- Reviews focus heavily on **action-oriented items**, with many reviews referring to LEGO sets for boys, such as cars, bikes, and action figures. 
- Reviews also emphasize themes like **building experiences** and the **quality/value** of LEGO products.

### Topic Analysis Insights
- **Topic 1**: LEGO sets for kids and general enjoyment.
- **Topic 5**: Bikes and minifigures connected with action-oriented themes.
- **Topic 9**: Nostalgic themes for fans and Vikings.
- Best number of topics identified by the **NMF model**: **11**.

## Visualization Analysis (TF-IDF)

### High TF-IDF Values
- Words like “item,” “expectation,” “nothing,” and “praise” had high TF-IDF scores, indicating their significance in distinguishing reviews.

### Low TF-IDF Values
- Many words had TF-IDF values close to 0, often due to their common usage across reviews, reducing their differentiation value.

#### Impact on Wordcloud
- The presence of many common words with TF-IDF values of 0 made the Wordcloud less effective in highlighting unique keywords or trends.

## Limitations & Observations

- **Data Bias**: The dataset is skewed toward LEGO products for boys, which could underrepresent products targeted at other demographics.
- **Repetitiveness in Themes**: Many topics are similar due to the dataset’s focus on LEGO-related products.
- **Positive Sentiment Dominance**: 76.92% of reviews were very positive, which could influence overall product perception.
