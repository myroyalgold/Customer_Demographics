# Customer_Demographics Data Cleaning

## Probelm Statement

## Problem Objectives
- Deal with irrelevant or inaccurate data
- Remove empty rows and duplicated data
- Change text case and date formatting
- Trim whitespaces from data
- Use Flash Fill and functions to clean data

# Dataset Used
  https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DA0130EN-SkillsNetwork/Hands-on%20Labs/Lab%205%20-%20Cleaning%20Data/Customer_demographics_and_sales_Lab5.xlsx

# Removing Duplicated, Irrelevant or Inaccurate Data
  ### Task A: Check spelling
  - Download the file Customer_demographics_and_sales_Lab5.xlsx.
  - Select column L (CREDITCARD_TYPE), then click Review tab, and select Spelling.
  - Click the correct suggestion to change the spelling for American Expres to American Express
  - Close the Spelling pane.

  ### Task B: Remove empty rows
  - Press CTRL+HOME, then press CTRL+SHIFT+END to select the whole datasheet.
  - On the Data tab, click Filter.
  - Click the Select All checkbox to deselect all of them. Then select just Blanks, then OK.
  - Select first row, then press CTRL+SHIFT+END to select all rows.
  - Right-click the selected rows and then click Delete Rows.
  - Finally, on the Data tab, click Clear, then click Filter.

  ### Task C: Remove duplicate rows
  - Select Column T (ORDER_ID) since ORDER_ID values are unique.
  - On the Home tab, click Conditional Formatting> Highlight Cells Rules> Duplicate Values, and then click OK.
  - Select the whole datasheet (CTRL+SHIFT+END)
  - On the Data tab, click Remove Duplicates.
  - In the Remove Duplicates dialog box, ensure that Select all columns is checked and that My data has headers is also checked, then click OK.
  - In the pop-up box informing you how many duplicate values were found and removed, click OK.
Note: There are 5 duplicate values found and removed; 194 unique
    


  
