# Milestone-1-2-and-3


The tasks outlined in the initial milestone involve various data processing and integration steps to ensure the coherence and quality of the dataset. Here's a breakdown of the key tasks:

Read Data:
Import data from each sheet of the Excel file into separate dataframes using the read_excel function.
Explore Data:
Use the head() function to preview the initial rows of each dataframe, providing an overview of the data.
Utilize the info() function to obtain a summary of each dataframe, including data types and non-null counts, which helps in understanding the structure and completeness of the data.
Analyze Dimensions:
For each dimension sheet (sheets starting with "Dim"), use the unique() function to identify unique keys within the respective dataframe.
Apply nunique() to count the number of unique keys for each dimension, providing insights into the cardinality of the data, which is crucial for understanding the uniqueness of dimension attributes.
Data Preprocessing Techniques:
Factsales and Dimpromotion Integration:

Merge Factsales and Dimpromotion based on the 'PromotionKey' to consolidate relevant information from both datasets seamlessly.
Data Fusion - DimSales and DimSalesperson:

Merge DimSales and DimSalesperson datasets to enhance the coherence of the combined information, likely using common keys like 'SalesPersonKey.'
Synergizing Dimstore and Fact Inventory:

Merge Dimstore and Fact Inventory datasets to create a merged DataFrame, possibly named as 'inv_store,' for enhanced clarity and consolidated inventory information.
Product Category and Product Subcategory Integration:

Merge Dimproduct category with Dimproductsubcategory using 'ProductCategoryKey' as the anchor to integrate critical datasets seamlessly.
Final Inventory Optimization:

Combine the result from the previous step with the 'inv_store' created earlier, merging with Dimproduct based on 'ProductSubcategoryKey' to optimize and enrich the inventory dataset, likely creating a DataFrame named 'final_inventory.'
Geographical Integration - Dimgeography and Final Inventory:

Forge a robust connection between Dimgeography and 'final_inventory' to ensure alignment of geographical attributes, likely using common keys such as 'GeographyKey.'
Customer and Enhanced Inventory Synthesis:

Bring together the Customer dataset with 'final_inventory' to intertwine customer-centric information with refined inventory data, likely merging based on customer-related keys.
By following these systematic steps, the dataset undergoes thorough preprocessing and integration, laying a strong foundation for subsequent analyses and strategic decision-making processes.
