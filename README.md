# Most Nutritious Starbucks Beverages - Power BI
A one page Power BI report that attempts to answer the question: "What are the most nutritious beverages on the menu?".\
Public Power BI Report Link: [here](https://www.novypro.com/project/most-nutritious-starbucks-beverages)

## Motivation
After seeing some submissions done by LinkedIn connections (on Linkedin obviously), I decided to try implementing my own report while improving some of the ideas that were done by others.\
Decided to create the report following the competition rules and constraints as well.\
All info regarding the competition rules and details can be found here: 

## Shortcomings
The unfortunate reality of having a one page constraint is that a lot of info had to be trimmed out.\
Additionally since the question is already specific, doing any additional data exploration adds unecessary info in this scenario.  

## Files 
The files found in this repository and their descriptions are as follows:
1. starbucks_beverage.csv: Dataset containing the info used for this report. Note that the dataset in not cleaned - the cleaning process was done in Power BI.
2. starbuckschallenge.pbix: The Power BI report. 

## Sample Screenshots
![Screenshot 2023-12-04 193243](https://github.com/splatterconstruct146/starbucks-nutrition-power-bi/assets/135209633/d295e525-1d18-4730-b8a3-ecbc9fe017cb)
Image 1: Overview page of the report. The report only has 1 page due to the competition constraints. 

## Process
Shows the process of creating the data table and then the report.
### 1. Cleaning the Data
There were some duplicate entries and mixed type columns (columns where entries where some were text, some were numbers).\
Decided to use median values for the duplicate entries (using a groupby to group the duplicates together). Note that this is not necessarily ideal - but it's better not to drop the duplicated entries altogether since these seem to be valid menu items (based on the menu item names).
The screenshot below exemplifies the cleaning process.\
![Screenshot 2023-12-05 191611](https://github.com/splatterconstruct146/starbucks-nutrition-power-bi/assets/135209633/965306f2-ce25-42ff-9078-1dc907424ce7)
Image 2: The right side of the screenshot shows the data transformations applied.

### 2. Applying a Shape Transformation to the Data
The radar chart visual requires the data to be pivoted to show the Attribute column and Value column.\
The screenshot below shows the steps and shape of the table for the radar chart.\
![Screenshot 2023-12-05 192108](https://github.com/splatterconstruct146/starbucks-nutrition-power-bi/assets/135209633/d95a1866-99a1-4640-9975-11f427a608cf)
Image 3: The right side of the screenshot shows how the shape of the table was changed. The contents are still the same.

### 3. Creating the Visuals
This step was fairly straightforward. Just apply the visuals that is best for representing the info in the data table. \

### 4. Applying a Visual Theme
Opted for something more aligned to the Starbucks branding. Thought it would be a good opportunity to practice some design skills as well.
