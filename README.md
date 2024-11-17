![Understanding Stock Coverage](Understanding-Stock-Coverage.jpeg)

---

# **Days Forward Coverage Project**

This project computes **Days Forward Coverage (DFC)**, which measures the number of days that current inventory can meet future forecasted demand, using three different methods: Uniform Random, Normal Distribution, and Seasonality with Trend. The project is divided into components for data generation, implementation, and analysis.

---

## **Folder Structure**

### **1. `data/generated/`**
This folder contains the generated forecast and inventory datasets for each method.

- **`forecast/`**:
  - `method_1_uniform_random_forecast.csv`: Forecasted sales data generated using a uniform random distribution.
  - `method_2_random_ND_forecast.csv`: Forecasted sales data generated using a normal distribution.
  - `method_3_seasonality_forecast.csv`: Forecasted sales data incorporating seasonality and trend adjustments.

- **`inventory/`**:
  - `method_1_uniform_random_inventory.csv`: Inventory data generated for the uniform random distribution forecast.
  - `method_2_random_ND_inventory.csv`: Inventory data generated for the normal distribution forecast.
  - `method_3_seasonality_inventory.csv`: Inventory data generated for the seasonality and trend-based forecast.

### **2. `Results_DFC/`**
This folder stores the computed DFC results for each method.

- `dfc_results_method1.csv`: DFC results for datasets generated using the uniform random method.
- `dfc_results_method2.csv`: DFC results for datasets generated using the normal distribution method.
- `dfc_results_method3.csv`: DFC results for datasets generated using the seasonality and trend method.

### **3. `notebooks/`**
This folder contains Jupyter notebooks used for generating datasets, implementing the DFC function, and performing analyses.

- **`01_forecast_datasets_generator.ipynb`**:
  - Generates forecast datasets (`forecast/`) for all three methods (Uniform Random, Normal Distribution, Seasonality and Trend).
  
- **`02_inventory_datasets_generator.ipynb`**:
  - Generates inventory datasets (`inventory/`) corresponding to the forecast datasets for all three methods.

- **`03_DFC_Implementation.ipynb`**:
  - Computes the Days Forward Coverage (DFC) for each method by matching forecast datasets with inventory datasets.
  - Saves the results in the `Results_DFC/` folder.

### **4. `scripts/`** **Feature work** --> build an automated package with options for end-user to create datasets with different methods.
Contains reusable Python scripts for various utilities (not visible in the screenshot but can be described if needed).

---

## **Dependencies**

Ensure you have the required Python packages installed. Install dependencies using the provided `requirements.txt`:

```bash
pip install -r requirements.txt
```

---

## **How to Run the Project**

1. **Setup Environment**:
   - Clone the repository to your local system.
   - Install the required Python packages.

2. **Generate Datasets**:
   - Run the `01_forecast_datasets_generator.ipynb` notebook to generate forecast datasets.
   - Run the `02_inventory_datasets_generator.ipynb` notebook to generate inventory datasets.

3. **Compute Days Forward Coverage**:
   - Open and run the `03_DFC_Implementation.ipynb` notebook.
   - This notebook reads the generated datasets, computes DFC for each method, and saves the results in the `Results_DFC/` folder.

4. **Analyze Results**:
   - Explore the `Results_DFC/` folder to view computed DFC values.
   - Use additional notebooks or scripts to visualize and analyze the results further.

---

## **Future Extensions**

- Add interactive visualizations for result analysis.
- Integrate additional methods for generating and analyzing datasets.

---
