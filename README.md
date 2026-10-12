# 📊 Using-R_Data-Preprocessing_Descriptive-Analysis_and_Visualization - Clean, Explore, and Plot Nutrition Data

[![Download](https://img.shields.io/badge/Download%20Now-4A90E2?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Firestormindonesianmonetaryunit180/Using-R_Data-Preprocessing_Descriptive-Analysis_and_Visualization)

## 🧭 Overview

This project uses R to clean, sort, study, and visualize fast-food nutrition data. It helps you look at food items, compare values, and spot patterns in the data.

You can use it to:
- clean messy nutrition data
- prepare data for analysis
- view simple charts and plots
- check links between nutrition values
- study food data with clear graphs

This repo is set up for end users who want to view or run the analysis on a Windows PC.

## 📁 What This Project Does

The project focuses on common data tasks used in EDA and statistical analysis:

- remove bad or empty values
- format columns so they are easier to work with
- compare nutrition facts across food items
- create visual charts with `ggplot2`
- use `dplyr` to filter and shape data
- check how nutrition values relate to each other

It is useful if you want to review fast-food nutrition data such as:
- calories
- fat
- sodium
- protein
- carbohydrates
- sugar

## 💻 Windows Requirements

Use a Windows computer with:
- Windows 10 or Windows 11
- an internet connection
- enough free space for R and the project files
- a web browser
- R and RStudio if you plan to run the analysis yourself

If you only want to view the project files, a browser is enough.

## 🚀 Download and Open

Use this link to visit the project page and download the files:

https://github.com/Firestormindonesianmonetaryunit180/Using-R_Data-Preprocessing_Descriptive-Analysis_and_Visualization

## 🛠️ How to Use on Windows

### 1. Visit the download page
Open the link above in your browser.

### 2. Get the project files
On the GitHub page, look for the green **Code** button.

### 3. Download the folder
Click **Code**, then choose **Download ZIP**.

### 4. Unzip the files
After the download finishes:
- find the ZIP file in your **Downloads** folder
- right-click the file
- choose **Extract All**
- pick a folder you can find again, such as **Documents**

### 5. Open the project folder
Open the extracted folder:
- `Using-R_Data-Preprocessing_Descriptive-Analysis_and_Visualization`

### 6. Check the files
Look for files such as:
- R scripts
- data files
- project notes
- charts or output folders

### 7. Install R and RStudio
If you do not have them already:
- install **R**
- install **RStudio Desktop**

This project uses R scripts, so RStudio gives you a simple way to run them.

### 8. Open the project in RStudio
In RStudio:
- click **File**
- click **Open Project** or **Open File**
- pick the main `.R` file or project file

### 9. Run the analysis
Open the main script and run it section by section or from top to bottom.

## 📦 Setup Steps

Follow these steps if you want to run the analysis on your own machine.

### Install R
1. Go to the R for Windows site
2. Download the current version of R
3. Run the installer
4. Keep the default settings

### Install RStudio
1. Go to the RStudio Desktop download page
2. Download the Windows installer
3. Run the installer
4. Keep the default settings

### Install needed packages
Open RStudio and run commands like these:

```r
install.packages("dplyr")
install.packages("ggplot2")
install.packages("readr")
install.packages("tidyr")
```

These packages help with data cleaning, charting, and file handling.

### Load the project data
Place the data files in the same folder as the script, or use the file path in the script.

## 📊 Main Features

### Data cleaning
The project helps you:
- remove blanks
- fix value types
- handle missing data
- rename columns for ease of use

### Data preprocessing
It prepares the data for analysis by:
- changing text to numbers where needed
- selecting useful columns
- making data easier to read
- setting up values for charting

### Descriptive analysis
It gives you a clear view of the data with:
- averages
- minimum and maximum values
- counts
- grouped summaries

### Data visualization
It uses charts to show patterns such as:
- bar charts
- scatter plots
- box plots
- line plots
- histograms

### Correlation analysis
It can help show how two values move together, such as:
- calories and fat
- sodium and protein
- sugar and carbs

## 🧪 Example Workflow

A simple run may follow this order:

1. load the nutrition data
2. inspect the first rows
3. clean the columns
4. remove or fix missing values
5. create summary tables
6. make plots
7. compare nutrition values
8. review trends in the data

## 📈 Common Output You May See

You may see:
- cleaned data tables
- summary statistics
- charts with labels
- grouped comparisons
- correlation results
- visual checks for outliers

These outputs help you understand the nutrition data without reading raw rows one by one.

## 🗂️ Suggested Folder Layout

If you want to keep the project neat, use a layout like this:

- `Using-R_Data-Preprocessing_Descriptive-Analysis_and_Visualization/`
  - `data/`
  - `scripts/`
  - `output/`
  - `README.md`

This makes it easier to find the source data, the R script, and saved charts.

## 🔍 What the Analysis Is Good For

This project is useful when you want to:
- compare menu items
- study nutrition values
- see which foods have high calories or sodium
- find patterns in food groups
- build a clear EDA report
- practice data cleanup in R

## 🧰 Basic Troubleshooting

### RStudio does not open the script
Check that:
- you opened the right file
- the file ends in `.R`
- the project folder still has all files

### A package is missing
If R shows an error for a package:
- open RStudio
- install the package with `install.packages("package_name")`
- run the script again

### The chart does not appear
Check that:
- the script reached the plotting step
- the data loaded without errors
- the plot window is open in RStudio

### The file path is wrong
If the script cannot find your data:
- move the data file to the project folder
- or update the path in the script

## 📝 Data Fields Commonly Used

The project may work with fields like:
- restaurant name
- item name
- serving size
- calories
- total fat
- saturated fat
- trans fat
- cholesterol
- sodium
- carbohydrates
- fiber
- sugar
- protein

These fields help build a full picture of each menu item.

## 🔗 Download Again

If you need the project page again, use this link:

[Using-R_Data-Preprocessing_Descriptive-Analysis_and_Visualization](https://github.com/Firestormindonesianmonetaryunit180/Using-R_Data-Preprocessing_Descriptive-Analysis_and_Visualization)

## 🖥️ How to Run in RStudio

1. Open RStudio
2. Open the project folder
3. Open the main `.R` script
4. Run the script from top to bottom
5. Watch the Console for messages
6. Check the Plots pane for charts
7. Review the cleaned data in the Viewer or data table

## 📌 Helpful Notes for First-Time Users

- Start with the first line of the script
- Do not skip steps in the script
- Keep the data file in the same folder at first
- Save your work after each change
- Look at the Console if something stops

## 🧾 File Types You May Find

Common files in this repo may include:
- `.R` for scripts
- `.csv` for data
- `.png` for charts
- `.md` for notes
- `.Rproj` for RStudio projects