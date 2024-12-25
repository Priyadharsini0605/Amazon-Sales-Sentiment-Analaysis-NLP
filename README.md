# Amazon Sales and Sentiment Analysis

## **Overview**
This project analyzes Amazon sales data to uncover insights into pricing trends, discounts, and customer sentiments. Using product reviews and pricing details, we extract actionable insights for categories, explore sentiment trends, and visualize correlations between pricing, discounts, and customer satisfaction.

---

## **Objectives**
1. **Pricing Analysis**:
   - Explore category-wise pricing and discount patterns.
   - Identify the effectiveness of discounts.

2. **Sentiment Analysis**:
   - Perform sentiment analysis on customer reviews.
   - Understand customer satisfaction levels for various categories.

3. **Insights and Recommendations**:
   - Identify key categories with high/low satisfaction levels.
   - Provide actionable insights to improve product offerings and customer satisfaction.

---

## **Technologies Used**
- **Python**: Data manipulation, analysis, and visualization.
- **Libraries**:
  - `pandas`, `numpy`: Data cleaning and analysis.
  - `matplotlib`, `seaborn`: Data visualization.
  - `TextBlob`, `WordCloud`: Sentiment analysis and word clouds.

---

## **Workflow**

### **Step 1: Data Loading**
The dataset was dynamically fetched from Kaggle using `kagglehub`:
```python
import kagglehub
path = kagglehub.dataset_download("karkavelrajaj/amazon-sales-dataset")
```

### **Step 2: Data Cleaning**
- Converted pricing columns (e.g., `discounted_price`, `actual_price`) to numeric formats.
- Handled missing and invalid values.

### **Step 3: Pricing and Discount Analysis**
- Calculated average pricing and discounts for each category.
- Visualized correlations between discounts, ratings, and prices using a heatmap.

### **Step 4: Sentiment Analysis**
- Performed sentiment analysis on customer reviews using `TextBlob`.
- Classified reviews as `Positive` or `Negative`.
- Generated a word cloud for positive reviews to highlight key customer preferences.

### **Step 5: Visualizations**
- Created stacked bar charts to visualize sentiment distribution across categories.
- Generated heatmaps to analyze correlations.

---

## **Key Insights**

### **Pricing and Discount Trends**:
1. **Category-Wise Analysis**:
   - Categories with higher discounts often have lower ratings, indicating potential quality concerns.
   - Top-performing categories (e.g., "Electronics") have balanced discounts and high ratings.

2. **Discount Effectiveness**:
   - Discounts do not always correlate positively with customer satisfaction.

### **Sentiment Analysis**:
1. **Sentiment Distribution**:
   - Overwhelmingly positive sentiments (~95%).
   - Categories with negative reviews often highlight quality or usability issues.

2. **Word Cloud Insights**:
   - Customers value **"quality," "ease of use,"** and **"product value."**
   - Positive sentiments align with attributes like "price," "durability," and "compatibility."

---

## **Visualizations**
### **1. Correlation Heatmap**
![Correlation Heatmap](path_to_heatmap.png)
- Highlights the relationship between discounts, ratings, and prices.

### **2. Sentiment Distribution**
![Sentiment Distribution](path_to_sentiment_distribution.png)
- Bar chart showing the proportion of positive and negative reviews.

### **3. Category-Wise Sentiment Distribution**
![Category Sentiment Distribution](path_to_category_sentiment.png)
- Stacked bar chart showing sentiment distribution across categories.

### **4. Word Cloud**
![Word Cloud](path_to_wordcloud.png)
- Key words and themes in positive reviews.

---

## **Future Enhancements**
1. **Advanced NLP Techniques**:
   - Use models like `VADER` or `BERT` for more granular sentiment analysis.

2. **Recommendation System**:
   - Build a system to recommend top products based on ratings and sentiments.

3. **Interactive Dashboards**:
   - Use tools like `Tableau` or `Power BI` to create dynamic visualizations.

---

## **Files in Repository**
1. **Code**:
   - `amazon_sentiment_analysis.ipynb`: Notebook containing all code.

2. **Dataset**:
   - Link to Kaggle: [Amazon Sales Dataset](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset).

3. **Visualizations**:
   - Heatmaps, bar charts, and word clouds for insights.

---

## **How to Run the Project**
1. Clone this repository.
2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn textblob wordcloud kagglehub
   ```
3. Run the notebook `amazon_sentiment_analysis.ipynb`.
4. Visualizations and insights will be generated in the output cells.

---

## **Conclusion**
This project demonstrates how to combine pricing analytics with sentiment analysis to derive actionable insights. It highlights the importance of aligning product quality and discounts with customer expectations to boost satisfaction and sales.

