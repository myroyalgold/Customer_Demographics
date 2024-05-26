# Customer_Demographics 

# Problem Statement
Data Cleaning

# Problem Objectives
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
Note: There are 5 duplicate values found and removed; 194 unique.
  
  ### Task D: Use Find & Replace to correct misspelling
  - On the Home tab, click Find & Select.
  - Click Find. In Find what, type jcb, and click Find All.
  - Click Replace
  - In Replace with, type JCB, click Replace All, and then click the Close icon.
  - On the Home tab, click Conditional Formatting> Clear Rules> Clear Rules from Entire Sheet.

# Dealing with Inconsistencies in Data
  ### Task A: Use the PROPER function to change text from upper case to proper case
  - Select row 2, then right-click it and choose Insert Rows.
  - In cell A2, type =PROPER(A1) and press Enter.
  - Hover over the bottom-right corner of cell A2, and drag the Fill Handle across to the last column.
  - If dragging across is too difficult with the mouse, then select the cells in the row 2 using SHIFT+RIGHT ARROW, then press F2 to put the cursor focus back in cell A2, then hold CTRL       while you press Enter.
  - Select row 2, then press CTRL+C.
  - Select row 1, Right-click and choose Paste Options>Values.
  - Select row 2, right-click it and choose Delete Rows.

  ### Task B: Use the UPPER function to change text from proper case to upper case
  - Select column AG (Generation). Then right-click and choose Insert Columns. In cell AG1, type Generation.
  - In cell AG2, type =UPPER(AH2) and press Enter.
  - Hover over the bottom-right corner of cell AG2 and double-click the Fill Handle.
  - Select column AG, then press CTRL+C.
  - Select column AH, right-click and choose Paste Options>Values.
  - Select column AG, right-click it and choose Delete Columns.

  ### Task C: Use the LOWER function to change text from proper case to lower case
  - Select column AC (T_Type). Then right-click and choose Insert Columns. In cell AC1, type T_Type.
  - In cell AC2, type =LOWER(AD2) and press Enter.
  - Hover over the bottom-right corner of cell AC2 and double-click the Fill Handle.
  - Select column AC, then press CTRL+C.
  - Select column AD, right-click and choose Paste Options>Values.
  - Select column AC, right-click it and choose Delete Columns.

  ### Task D: Change date formatting
  - Select column Z (Order_Ship_Date).
  - On the Home tab, in the Number group click Number Format> More Number Formats.
  - In the Category list, select Date.
  - In the Format Cells box, under Locale, select English (United States).
  - Under Type, select Wednesday, March 14, 2012 and click OK.

  ### Task E: Use Find & Replace to trim whitespace
  - Click CTRL+HOME.
  - Select all the data using CTRL+SHIFT+END.
  - On the Home tab, click Find & Select, then Replace.
  - In Find what, type 2 spaces. In Replace with, type 1 space.
  - Click Find All, then click Replace All.
  - Click the Close icon.

# More Excel Features for Cleaning Data
  ### Task A: Use the Flash Fill feature to clean data:
  - Select column A (Cust_Name), right-click and choose Insert Columns.
  - In cell A1 type Customer_Name and press Enter.
  - In cell A2, type Mr. Allen Perl and press Enter.
  - Select column A (Customer_Name), on the Data tab, click Flash Fill.
  - Click Undo to undo this step.

  ### Task B: Use LEFT, RIGHT, LEN, and SEARCH functions to clean data:
  - Select column A (Cust_Name), right-click and choose Insert Columns.
  - Select column A again, right-click and choose Insert Columns.
  - In cell A1, type Customer_Firstname and in cell B1, type Customer_Lastname.
  - Click C1, then on the Home tab, click Format Painter, then drag across to A1 and B1.
  - Double-click the divider between columns A and B.
  - In cell A2 type =LEFT(C2, SEARCH(“ “,C2,1)) and press Enter.
  - In cell B2 type =RIGHT(C2,LEN(C2)-SEARCH(“ “,C2,1)) and press Enter.
  - Double-click the Fill Handle on cell A2.
  - Double-click the Fill Handle on cell B2.
  
