
# **📊 Data Catalog for Gold Layer**

  

The **Gold Layer** is the business-level data representation, structured to support **analytical and reporting use cases**. It consists of **dimension tables** and **fact tables** designed to capture and serve specific business metrics.

----------

### 1. gold.dim_customers

**Purpose**:
Stores customer details enriched with **demographic** and **geographic** data.

**📁 Columns**
| Column Name | Data Type | Description
|--|--|--
|customer_key|INT|Surrogate key uniquely identifying each customer record in the dimension table.
|cutomer_id|INT|Unique numerical identifier assigned to each customer.
|customer_number|NVARCAHR(50)| Alphanumeric identifier representing the customer, used for tracking and referencing.
|first_name|NVARCHAR(50)| The customer’s first name, as recorded in the system.
|last_name|NVARCHAR(50)|The customer’s last name or family name.
|country|NVARCHAR(50)|The country of residence for the customer *(e.g., ‘Australia’)*.
|marital_status|NVARCAHR(50)| The marital status of the customer (e.g., _‘Married’_, _‘Single’_).
|gender|NVARCHAR(50)| The gender of the customer (e.g., _‘Male’_, _‘Female’_, _‘n/a’_).
|birthdate|DATE| The date of birth of the customer, formatted as YYYY-MM-DD (e.g., 1971-10-06).
|create_date|DATE| The date and time when the customer record was created in the system.

----------
### 2. gold.dim_products

**Purpose**:
Provides detailed information about **products** and their **attributes**.

**📁 Columns**
| Column Name | Data Type | Description
|--|--|--
|product_key|INT|Surrogate key uniquely identifying each product record in the product dimension table.
|product_id|INT|Unique identifier assigned to the product for internal tracking and referencing.
|product_number|NVARCHAR(50)|Structured alphanumeric code representing the product, often used for categorization or inventory.
|product_name|NVARCHAR(50)|Descriptive name of the product, including key details such as type, color, and size.
|category_id|NVARCHAR(50)|Unique identifier for the product’s category, linking to its high-level classification.
|category|NVARCHAR(50)|Broader classification of the product (e.g., _Bikes_, _Components_).
|subcategory|NVARCHAR(50)|More detailed classification of the product within the category.
|maintenance_required|NVARCHAR(50)|Indicates whether the product requires maintenance (e.g., _‘Yes’_, _‘No’_).
|cost|INT|Cost or base price of the product, measured in monetary units.
|product_line|NVARCHAR(50)|Specific product line or series (e.g., _Road_, _Mountain_).
|start_date|DATE|Date when the product became available for sale or use.

---------
### 3. gold.fact_sales

**Purpose**:
Stores **transactional sales data** for detailed **analytical** purposes.

 **📁 Columns**
 | Column Name | Data Type | Description
|--|--|--
|order_number|NVARCHAR(50)|Unique alphanumeric identifier for each sales order (e.g., _‘SO54496’_).
|product_key|INT|Surrogate key linking the order to the product dimension table.
|customer_key|INT|Surrogate key linking the order to the customer dimension table.
|order_date|DATE|The date when the order was placed.
|shipping_date|DATE|The date when the order was shipped to the customer.
|due_date|DATE|The date when the order payment was due.
|sales_amount|INT|Total monetary value of the sale, in whole currency units (e.g., 25).
|quantity|INT|Number of units of the product ordered (e.g., 1).
|price|INT|Price per unit of the product for the line item, in whole currency units.
