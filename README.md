# laptop-price-predictor-ML

The Laptop Price Predictor project leverages machine learning to predict the price of laptops based on their specifications. This tool helps consumers, retailers, and manufacturers make informed decisions about laptop pricing and purchasing.

## Overview

The Laptop Price Predictor project uses machine learning to estimate laptop prices based on their specifications. It helps users, retailers, and manufacturers make informed pricing and purchasing decisions through an easy-to-use interface that provides real-time price predictions and insights into the factors influencing laptop prices.

## Setup

To run this project locally, follow these steps:

1. ### Clone the Repository

```sh
git clone https://github.com/Aja-creator/laptop-price-predictor-ML.git
cd laptop-price-predictor-ML
```





2.  ### Create and Activate a Virtual Environment 
	Using venv (for Python 3.x) 
	#### Create a virtual environment 
	```bash
	 # Create a virtual environment named 'venv'
	  python3 -m venv venv
	  ```
    ####  Activate the Virtual Environment 
    ##### On Windows 
    ```bash 
    .\env\Scripts\activate
    ```
    ##### on macOS
     ```bash
      source env/bin/activate
      ```
3. ### Install dependencies

    Ensure you have Python 3.x installed along with the necessary libraries. Install them using:

    ```bash
    pip install pandas nltk scikit-learn
    ```

    You also need to download NLTK data:

    ```bash
	python -m nltk.downloader wordnet
	```

4.  ### Download the dataset

    -   Download the laptop_data dataset 
    -   Place the `laptop_data.csv`  file in a directory accessible to your Python environment.
5.  ### Run the preprocessing script

    Execute the model builder script (`laptop_price_predictor_ML.ipynb` or similar) in Google Colab or Jupyter notebook
    This script cleans the data, extracts relevant features, applies lemmatization, and computes TF-IDF vectors .

6.  ### Run the prediction system:

    Start the Streamlit application:

    ```bash
	streamlit run app.py
	```

    Open a web browser and navigate to `http://localhost:8501` to access the prediction system.

## Usage
 

 -  **Select the Brand:** Choose the laptop brand from the dropdown menu.
 -  **Select the Type:** Choose the laptop type from the dropdown menu.
 -  **Enter the Processor Type:** Input the type of processor (e.g., Intel i5, AMD Ryzen 7).
 -  **Enter the RAM Size:** Input the size of the RAM in GB.
 -  **Enter the Storage Type:** Choose the type of storage (e.g., SSD, HDD) from the dropdown menu.
 -  **Enter the Storage Capacity:** Input the storage capacity in GB .
 -  **Select the GPU:** Choose the graphics processing unit from the dropdown menu.
 -  **Enter the Screen Size:** Input the screen size in inches.
 -  **Enter the Resolution:** Input the screen resolution (e.g., 1920x1080).
 -  **Select the Operating System:** Choose the operating system from the dropdown menu.
 -  **Predict Price:** Click the button to view the predicted price for the laptop based on the input specifications.
