#  Customer Segmentation Using RFM Analysis  

This project performs **Customer Segmentation using RFM (Recency, Frequency, Monetary) Analysis** on the famous **Online Retail Dataset (UCI)**.  
It’s a practical way to identify different customer groups and create targeted marketing strategies.  



##  Project Overview  

The project follows these steps:  

1. **Load & Clean Data**  
   - Removed canceled orders.  
   - Dropped missing Customer IDs and Descriptions.  
   - Removed negative quantities and zero prices.  
   - Converted `InvoiceDate` to datetime.  
   - Added `TotalPrice` column (Quantity × UnitPrice).  

2. **Calculate RFM Metrics**  
   - **Recency** → Days since last purchase.  
   - **Frequency** → Number of purchases.  
   - **Monetary** → Total spending.  

3. **Score Customers**  
   - Scored Recency, Frequency, and Monetary on a 1–4 scale.  
   - Combined into a single `RFM_Score`.  

4. **Segment Customers**  
   - Segmented into groups like **Champions**, **Loyal Customers**, **At Risk**, **Lost Customers**, etc.  

5. **Visualizations**  
   - Bar chart of customer segments.  
   - Heatmap of average RFM values per segment.  

6. **Marketing Ideas (Step 7)**  
   - Each segment is linked to actionable marketing strategies (see below).  



##  Marketing Ideas Based on Segments  

**Champions** → Reward them with loyalty programs, exclusive offers, and early product launches.  

**Loyal Customers** → Encourage referrals, give them early access to sales, and upsell/cross-sell.  

**Potential Loyalist** → Offer discounts for second purchase, nurture them into loyal customers.  

**New Customers** → Welcome them with onboarding emails, small discounts, and product recommendations.  

**At Risk** → Send win-back campaigns, discounts, and reminders about what they loved before.  

**Lost Customers** → Try re-engagement campaigns or surveys to understand why they left.  

 



##  Visuals  

- **Segment Count Plot** → Shows how many customers belong to each segment.  
- **Heatmap** → Displays average Recency, Frequency, and Monetary for each segment.  



##  Technologies Used  

- **Python**  
- **Pandas**  
- **Matplotlib**  
- **Seaborn**  
- **Jupyter Notebook**  



##  Files in this Repository  

- `RFM_Analysis.ipynb` → Jupyter Notebook with full analysis.  
- `README.md` → This file.  
- `Online Retail Dataset` → (Download from UCI Machine Learning Repository).  



##  How to Run  

1. Clone the repository.  
2. Install required libraries:  

```bash
pip install pandas matplotlib seaborn openpyxl
