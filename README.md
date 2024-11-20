# Athletic Sales Analysis
# Data Analysis Project: Sales Insights  

This Python program analyzes sales data to generate insights about the top-performing regions, retailers, and product categories. The program also identifies peak sales periods for women's athletic footwear.  

## Features  

### 1. **Data Cleaning and Preparation**  
- Combines two datasets into a single DataFrame using an inner join and resets the index.  
- Converts the `invoice_date` column to a datetime data type for time-based analysis.  

### 2. **Top Regions by Product Sales**  
- Aggregates sales data using `groupby` or `pivot_table` to create a multi-index DataFrame (`region`, `state`, and `city`).  
- Renames the aggregated column for clarity.  
- Sorts results in descending order to display the top five regions based on product sales.  

### 3. **Top Regions by Total Sales Revenue**  
- Uses `groupby` or `pivot_table` to aggregate revenue data for `region`, `state`, and `city`.  
- Renames the aggregated column to clarify the data representation.  
- Displays the top five regions by sales revenue.  

### 4. **Top Retailers by Total Sales Revenue**  
- Aggregates revenue data by `retailer`, `region`, `state`, and `city` using `groupby` or `pivot_table`.  
- Renames the aggregated column for better interpretation.  
- Displays the top five retailers and their respective locations by total sales revenue.  

### 5. **Top Retailers for Women's Athletic Footwear**  
- Filters the dataset to include only women's athletic footwear sales.  
- Uses `groupby` or `pivot_table` to aggregate sales data for `retailer`, `region`, `state`, and `city`.  
- Renames the aggregated column and sorts the results to identify the top five retailers for this category.  

### 6. **Day with the Most Women's Athletic Footwear Sales**  
- Creates a pivot table with `invoice_date` as the index and `total_sales` as the value.  
- Resamples the data to daily intervals and calculates the total daily sales.  
- Displays the days with the highest sales.  

### 7. **Week with the Most Women's Athletic Footwear Sales**  
- Resamples the daily sales data into weekly intervals.  
- Identifies the weeks with the highest women's athletic footwear sales.  

## Requirements  

- Python 3.7 or later  
- Pandas library for data manipulation  
- Jupyter Notebook (optional for interactive analysis)  

## Installation  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-repo/sales-analysis.git  
   cd sales-analysis  
   ```  

## Usage  

1. Run the script:  
   ```bash  
   python main.py  
   ```  
2. Follow the output to view insights for each task described above.  

## File Structure  

- **`data/`**: Contains input datasets  
- **`main.py`**: Main script for analysis  
- **`output/`**: Directory for saving analysis results  


## Contributing  

Feel free to contribute by submitting a pull request or raising issues for any bugs or feature requests.  

## License  

This project is licensed under the MIT License. See the `LICENSE` file for details.  

## Acknowledgments

This project was developed with the assistance of ChatGPT, an AI language model created by OpenAI. The model helped in generating ideas, code snippets, and documentation to enhance the overall development process.
