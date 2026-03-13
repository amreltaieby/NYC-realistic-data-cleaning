My first realistic project after about **1–2 weeks of studying Pandas**.
This project focuses on **cleaning and preparing a real estate dataset** so it can be used for later analysis or visualization.

The goal was to practice **data manipulation, feature engineering, and handling missing values** in a structured way.

---

## Features of this Project

### Created Features

#### SQFT Related

* **Price per square foot for each property**
* **Market average price per square foot in New York**
* **Average room size (square feet per room)**

#### Additional Columns

* **Room Count**
  Aggregates all room-related attributes:

  beds + full bathrooms + garage spaces

* **Price per Sqft**
  Calculated for every listing to standardize property comparison.

* **Market Value Classification**
  Each property is categorized based on its price per square foot relative to the NYC market average:

  * Above Market Value
  * Below Market Value
  * At Market Value

---

### Cleaning Unrealistic Rows

The dataset is filtered to remove unrealistic or invalid listings, including:

* Extremely low or extremely high prices
* Unrealistic square footage values
* Invalid bedroom or bathroom counts
* Impossible garage values
* Invalid price-per-square-foot values
* Unrealistic total room counts

This ensures the final dataset contains **reasonable real estate listings**.

---

### Filling Missing Data (Main Focus of the Project)

The main focus of this project is **handling missing values using dataset-derived estimates**.

Missing values were filled using calculated averages from the dataset.

Filled columns include:

* **sqft**
  Estimated using:

  room_count × average_sqft_per_room

* **stories**
  Estimated using:

  room_count ÷ average_rooms_per_story

* **garage**
  Missing values defaulted to **1 garage space**.

* **price_per_sqft**
  Any remaining missing values were filled using the **overall market average price per square foot**.

---

### Output

The cleaned dataset is exported as:

NYC_dataset_cleaned_Amr_Eltaieby.csv

This dataset is ready for:

* exploratory data analysis (EDA)
* visualization
* machine learning models

---

## Skills Practiced

* Pandas data manipulation
* Boolean filtering
* Handling missing data
* Feature engineering
* Data validation
* Dataset export

---

## Future Improvements

Possible next steps for this project:

* Data visualization (Matplotlib / Seaborn)
* Exploratory data analysis (EDA)
* Outlier detection using statistical methods
* Price prediction models using machine learning




note : chat gpt & VS code assitant were used but mainly for syntax and to learn new things then written again alone.
