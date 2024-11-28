# Shopping Trends Dashboard

## Problem Statement

This dashboard provides insights into shopping trends and customer behaviors to help businesses enhance their retail strategies. It enables companies to:

### Understand Customer Preferences:
- Analyze purchasing patterns based on age, gender, and geographic location.
- Identify the most popular product categories and seasons for purchases.

### Evaluate Performance Metrics:
- Assess the effectiveness of promotional strategies through metrics like discount usage and promo code applications.
- Examine customer feedback using review ratings to identify areas for improvement.

### Optimize Operations:
- Analyze shipping preferences to refine logistics strategies.
- Evaluate the impact of subscription status on customer retention and purchasing frequency.

### Address Key Challenges:
- Improve customer satisfaction by addressing low review ratings (average rating ~3.1 across items).
- Enhance product offerings in categories with high dissatisfaction rates or fewer purchases.

The dataset also highlights the importance of seasonal strategies, payment method preferences, and discount-driven sales, guiding businesses to create tailored marketing campaigns and improve operational efficiency.

---

## Steps Followed  

### 1. Prepare Your Data  
1. **Open Power BI Desktop**  
2. **Load the Data**:  
   - Click on **"Get Data"**.  
   - Select the file format (e.g., Excel, CSV), and load your `shopping_trends.csv` file.  
3. **Clean and Transform the Data**:  
   - Open the **Power Query Editor** by clicking on **"Transform Data"**.  
   - Remove unnecessary columns.  
   - Rename columns for clarity (e.g., `ID` → `Customer ID`).  
   - Handle missing or inconsistent data (e.g., replace null values).  
4. **Create Calculated Columns or Measures** (if required):  
   - **Total Purchase Amount**: `Sum(Purchase Amount)`  
   - **Average Review Rating**: `Average(Review Rating)`  

---

### 2. Design the Layout  
1. **Set the Theme**:  
   - Go to the **View** tab.  
   - Apply a pre-built theme or create a custom theme (e.g., pink and purple for the dashboard).  
2. **Add a Background (Optional)**:  
   - Insert a custom image or set a plain-colored background to improve aesthetics.  

---

### 3. Create Visuals  

#### Key Metrics (Cards)  
- **Steps**:  
  1. Click on the **Card Visual** from the Visualizations pane.  
  2. Drag measures like `Sum of Purchase Amount` into the **Fields** pane.  
  3. Create the following cards:  
     - **Total Purchase Amount**: $233K  
     - **Average Review Rating**: 3.75  
     - **Total Customers**: 3900  
  4. Format the cards by adjusting the font size, color, and alignment.  

#### Line Chart for Age Trends  
- **Steps**:  
  1. Select the **Line Chart** visual.  
  2. Drag `Age` to the **X-axis** and `Count of Customer ID` to the **Y-axis**.  
  3. Add data points and customize the line color to purple.  

#### Bar Chart for Location and Products  
- **Steps**:  
  1. Choose the **Clustered Bar Chart** visual.  
  2. Drag `Location` to the **Y-axis** and `Count of Customer ID` to the **X-axis**.  
  3. Create a second bar chart for `Items Purchased` by `Customer Count`.  
  4. Format the bars by changing colors and enabling data labels.  

#### Area Chart for Seasonal Trends  
- **Steps**:  
  1. Select the **Area Chart** visual.  
  2. Drag `Season` to the **X-axis** and `Sum of Purchase Amount` to the **Y-axis**.  
  3. Format the chart with a gradient purple fill.  

---

### 4. Add Slicers for Filters  
- **Steps**:  
  1. Add slicers for:  
     - **Shipping Type**  
     - **Size**  
     - **Color**  
     - **Gender**  
     - **Category**  
  2. Link slicers to all visuals by enabling **Edit Interactions** in the Format ribbon.  
  3. Customize the slicer style as dropdowns or horizontal buttons.  

---

### 5. Customize and Format  
- **Steps**:  
  1. Open the **Format Pane** for each visual.  
  2. Adjust:  
     - Titles (e.g., "Count of Customers by Age").  
     - Background colors and transparency.  
     - Borders for visuals.  
  3. Add **dynamic titles** using measures or fields (e.g., "Filtered by: [Category]").  

---

### 6. Test the Interactivity  
- Apply different slicer filters to ensure visuals respond dynamically.  
- Check cross-filtering between visuals (e.g., selecting "Blouses" updates other charts).  

---

### 7. Publish and Share  
1. **Save and Publish**:  
   - Save the Power BI file (`.pbix`).  
   - Publish to the **Power BI Service** by signing into your account.  
2. **Create a Dashboard in Power BI Service**:  
   - Pin visuals from the report to a dashboard.  
   - Add alerts or subscriptions for real-time updates.  

---

## Key Tips  
- Use **consistent colors** for similar data points across visuals.  
- Keep the layout clean and organized for better readability.  
- Use **tooltips** to show additional information when users hover over visuals.  
- Leverage Power BI’s **Drill Through** feature to navigate between detailed reports.  

---

### Example Visuals  
- **Cards**: Highlight total purchase amount, average rating, and total customers.  
- **Line Chart**: Show trends by age.  
- **Bar Chart**: Display location and product distribution.  
- **Area Chart**: Represent seasonal purchase trends.  

---

By following these steps, you can create an interactive and visually appealing **Shopping Trends Dashboard** to gain insights into your data.

![Shopping_trands_page-0001](https://github.com/user-attachments/assets/f16ca2a0-abaf-4be5-9fb9-ef91320fdf4d)
