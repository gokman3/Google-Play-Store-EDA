# Google Play Store Apps Data Analysis 📱

## Overview

This project performs Exploratory Data Analysis (EDA) on the Google Play Store Apps dataset. The goal is to derive insights into the Android app market, analyzing trends in app categories, ratings, size, and pricing strategies.

## 📂 Dataset

The dataset contains details of approximately 10,000 Android applications.

  * **Source**: [Google Play Store Apps Dataset](https://www.kaggle.com/lava18/google-play-store-apps)
  * **Key Features**: App Name, Category, Rating, Reviews, Size, Installs, Type, Price, Content Rating, Genres, etc.

## 🛠️ Technologies Used

  * **Language**: Python
  * **Libraries**:
      * `pandas` (Data manipulation)
      * `numpy` (Numerical operations)
      * `matplotlib` & `seaborn` (Data visualization)

## 🧹 Data Cleaning & Preparation

Before analysis, the raw data required significant preprocessing:

1.  **Handling Missing Values**:
      * Filled missing `Rating` values with the median.
      * Dropped records with missing `Content Rating`, `Current Ver`, and `Android Ver`.
2.  **Data Type Conversion**:
      * Converted `Reviews` to numeric.
      * Processed `Size`: Converted "M" (Megabytes) and "k" (kilobytes) to a standard float format.
      * Processed `Installs`: Removed "+" and "," characters to convert to numeric.
      * Processed `Price`: Removed "$" symbols to convert to numeric.
      * Converted `Last Updated` to datetime format.
3.  **Removing Duplicates**: Dropped duplicate entries based on App Name.

## 📊 Key Analysis & Visualizations

The notebook includes various visualizations to understand the data distribution:

  * **Category Analysis**: Count plots showing the most popular app categories (e.g., Family, Game, Tools).
  * **Rating Distribution**: Histograms showing the spread of app ratings (mostly skewed towards 4.0 - 5.0).
  * **Installs & Reviews**: Log-transformed distribution plots to analyze user engagement.
  * **Pricing Strategy**: Analysis of Free vs. Paid apps.
  * **Genres**: Detailed breakdown of app genres.

## 🚀 How to Run

1.  Clone this repository.
2.  Install the required libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
3.  Open the notebook `EDA_GooglePlayStore.ipynb` in Jupyter Notebook or Google Colab.
4.  Ensure the `googleplaystore.csv` file is in the correct path specified in the notebook.

## 👤 Author

**Gökmen Balcı**

-----

### Step 3: The "About" Section (Sidebar)

On the right side of your repository page, you will see an **About** section with a gear icon. Click it and add:

  * **Description**: Exploratory Data Analysis and cleaning of Google Play Store data using Python (Pandas/Seaborn).
  * **Topics**: `python`, `data-analysis`, `eda`, `pandas`, `visualization`
