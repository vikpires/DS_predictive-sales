# Predictive sales using Azure Machine Learning

> Challenge created as part of the Microsoft Certification Challenge #3 DP-100 Bootcamp by DIO:

## Scenario
Imagine that you own an ice cream shop called Gelato Magic in a seaside town. You know that the amount of ice cream you sell each day is strongly correlated with the ambient temperature. However, without proper planning, you may end up producing more ice cream than necessary and incur losses due to waste, or conversely, produce less and lose sales.

To solve this problem, you decide to use machine learning to predict how much ice cream will be sold based on temperature. With this model, you can anticipate demand and plan production efficiently.

## Goal

The objective of this project is to develop a predictive regression model that allows:

✅ Train a Machine Learning model to predict ice cream sales based on the day's temperature.

✅ Register and manage the model using MLflow.

✅ Implement the model for real-time forecasting in a cloud computing environment.

✅ Create a structured pipeline to train and test the model, ensuring reproducibility.

---

## 1. Creating the database

To create the database was used a prompt in Copilot as below:

```
Create a sample database with 100 rows simulating ice cream sales based on date, sales, and temperature. The spreadsheet should be in CSV format.
```
The CSV file **gelato_database** can be found in the folder <a href= './inputs'>input</a>. 

<br />

**Ice Cream Sales Data Summary**

| Date       | Sales (units) | Temperature (°C) |
|------------|---------------|-------------------|
| 2025-01-01 | 150           | 25                |
| 2025-01-02 | 120           | 23                |
| 2025-01-03 | 180           | 28                |
| 2025-01-04 | 140           | 26                |
| 2025-01-05 | 160           | 27                |
|    ...     | ...           | ...               |

## 2. Setting the environment in Azure Machine Learning

### 2.1. Create a project in Azure Machine Learning

- Start by provisioning an Azure Machine Learning workspace in the Azure portal.

- Search for *Machine Learning* in the Azure portal and create a new Azure Machine Learning resource.

- Navigate to the Azure Machine Learning Studio to manage your machine learning resources.

- In Azure Machine Learning Studio, select the *Compute* option and set a **compute instance** and **compute cluster**.

- Now, select *Notebooks*. Create a folder, upload the data and create a new notebook.


