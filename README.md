
Edunet Internship - Personal Carbon Footprint Predictor (Week 1)

### About This Project
This repository is my Week 1 submission for the AICTE "AI with Green Energy" internship.

The task for this week was to:
1.  Find and collect relevant data for our "Energy (Prediction)" theme.
2.  Perform **Data Cleaning** (fixing missing values).
3.  Perform **Data Pre-processing** (combining files, engineering new features).

The final dataset (`final_carbon_footprint_dataset.csv`) is now 100% numeric and ready for an AI model.

---

## Files in this Repository

### 1. `final_carbon_footprint_dataset.csv`
* **What it is:** This is the **final, clean dataset** for the project.
* **Total Rows:** 19,735
* **How I made it:** I combined two different datasets (UCI Household Energy and UCI Auto MPG). I cleaned the missing values from the MPG data and then pre-processed both to create a single, rich dataset.

### 2. `dataset1.ipynb`
* **What it is:** This is the **Google Colab "recipe" file**.
* **Why it's here:** It contains all the Python code (Steps 1-5) that shows the *exact process* of how I loaded the raw data, cleaned it, and engineered the final CSV file. It's the proof of the pre-processing work.

---

## Data Dictionary (What's in the CSV)
This explains what each (all-numeric) column means:

* `home_energy_wh`: Total energy used by the house (in Wh).
* `outside_temp_C`: Outside temperature (in Celsius).
* `vehicle_mpg`: The mileage (MPG) of the car used for that day.
* `vehicle_weight`: The weight (in lbs) of the car used.
* **`total_carbon_impact` (TARGET):** This is the calculated "carbon score" that we will train our AI model to predict.
