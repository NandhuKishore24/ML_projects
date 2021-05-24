Main Notebook File - PCAM ZC321-C3-CODE-USEDCARPRICEPREDICTION-G7.ipynb
	Input files     - vehicles.csv (Raw Dataset)
	Output files	- vehicles_db1.csv (Data after imputation of missing values performed using column match)
					- vehicles_db2.csv (Data after extraction of new columns, removal of existing columns, data correction and removal of all the rows having atleast one null values other than odometer)
					- vehicles_db3.csv (Data after refined values of price and odometer and also normalized odometer column)
					- vehicles_db4.csv (Data after Target encoding, ordinal encoding, scaling of features and KNN imputation for Odometer missing values)
					- vehicles_db5.csv (Dataset in which outliers are removed using DBscan)
					- vehicles_db6.csv (Dataset in which outliers are removed using ZScore)

Notebook Files for ML Models
1. PCAM ZC321-C3-CODE-USEDCARPRICEPREDICTION-G7-MODELS_1.ipynb
	Input files     - vehicles_db4.csv (Dataset without removing any outliers)
	Output files 	- metrics_outliers.csv (csv file with metrics for all the algorithms trained)

2. PCAM ZC321-C3-CODE-USEDCARPRICEPREDICTION-G7-MODELS_2.ipynb
	Input files 	- vehicles_db5.csv (Dataset in which outliers are removed using DBscan)
	Output files 	- metrics_dbscan.csv (csv file with metrics for all the algorithms trained)

3. PCAM ZC321-C3-CODE-USEDCARPRICEPREDICTION-G7-MODELS_3.ipynb
	Input files 	- vehicles_db6.csv (Dataset in which outliers are removed using ZScore)
	Output Files 	- metrics_zscore.csv (csv file with metrics for all the algorithms trained)

Steps to Run
1. Start running the PCAM ZC321-C3-CODE-USEDCARPRICEPREDICTION-G7.ipynb file until Model Metrics section.
2. Make sure the listed csv files are created in the directory
3. Run the ML model notebooks one by one and check for the ouput metrics csv files
4. Run the Model Metrics section in the PCAM ZC321-C3-CODE-USEDCARPRICEPREDICTION-G7.ipynb notebook to check the consolidated metrics

Note: We can directly run the ML model notebooks by placing the corresponding input csv files.