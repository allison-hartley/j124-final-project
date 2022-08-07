# J124 Final Project: 
## By Allison Hartley

## Acquiring and Cleaning the Data
* Go to the UC Office of the President Website and navigate to Organization -> Financial Accounting -> Financial Reports -> [Campus Financial Schedules](https://www.ucop.edu/financial-accounting/financial-reports/campus-financial-schedules/index.html). Download the PDF file for Berkeley for the past five fiscal years: [2019-2020](https://www.ucop.edu/financial-accounting/financial-reports/campus-financial-schedules/19-20/berkeley.pdf), [2018-2019](https://www.ucop.edu/financial-accounting/financial-reports/campus-financial-schedules/18-19/berkeley.pdf), [2017-2018](https://www.ucop.edu/financial-accounting/financial-reports/campus-financial-schedules/17-18/berkeley-consolidated.pdf), [2016-2017](https://www.ucop.edu/financial-accounting/financial-reports/campus-financial-schedules/16-17/berkeley-consolidated.pdf), and [2015-2016](https://www.ucop.edu/financial-accounting/financial-reports/campus-financial-schedules/15-16/berkeley-consolidated.pdf).
* Use an optical character recognition (OCR) program such as [Tabula](https://tabula.technology/) to convert the PDF to Excel. 
* Extract the tables for Instruction funding for the major UC Berkeley colleges, including the College of Engineering, School of Business Administration, College of Chemistry, School of Education, Graduate School of Journalism, School of Law, College of Letters and Science, School of Information Management, College of Natural Resources, School of Optometry, School of Public Health, Graduate School of Public Policy, and School of Social Welfare. Include department breakdowns when available. 
* Clean the data by standardizing department names with title case in Open Refine, formatting values as dollar amounts, and consolidating the data into one worksheet.
* Use the VLOOKUP formula to match up the department names with their funding in one spreadsheet.
* Find errors and manually check and fix the data entries. Some department names may not be adequately parsed by OCR, causing inaccuracies.
* Make the data easier to read by putting college names in bold and freezing the first column and rows up to the year.
<br> <p align="left"> *Partial screenshot of cleaned data:*
<p align="center">
<img width="812" alt="Cleaned data showing Instructional Funding over school years from 2015-2020 for major colleges within UC Berkeley." src="https://user-images.githubusercontent.com/32043036/183220826-6ef5877d-7ea3-40f8-8187-0a0a8e2a7c66.png">
<br> 

## Interrogating the Data
Before manipulting the data, duplicate the cleaned data set to refer to later in case of mishaps. Conduct analysis on a copy of the cleaned data. 
### Which school had the greatest increase in funding between 2015 and 2020? 
1. Let's answer this question using percent change to give a fair comparison of changes over time between departments of different sizes. 
2. Add a new column called "Percent Change Between 15-16 and 19-20," and type "=" to enter the function for percent change: (New - Old)/(Old). 
  <p align="center"> 
  <img width="1049" alt="Screenshot of one row, showing the cell entry for percent change. The departments' 2015-2016 funding are subtracted from 2019-2020 data, and the result is divided by the 2019-2020 funding." src="https://user-images.githubusercontent.com/32043036/183222140-a5ef2b47-12c8-4449-95c9-c63cd40a260e.png">
<p align="left"> 3. Repeat the formula for all rows with funding data by dragging the bottom right corner of the cell down the column. 
<br>4. Click the percent button to format the column as a percent. Use the buttons to the right to decrease or increase decimal places.
<p align="center"> 
 <img width="758" alt="Screenshot pointing to the buttons for formatting as a percent and increasing/decreasing decimal points." src="https://user-images.githubusercontent.com/32043036/183222987-02de1439-ffb8-423c-bfd1-0a5d27096795.png">
<br> <p align="left"> 5. Turn on filters. In the college/department column, click "Clear," then select the schools/colleges we're interested in. 
 <p align="center">  <img width="535" alt="Screenshot showing filter settings for the first column. Clear selections, then choose only the colleges of interest." src="https://user-images.githubusercontent.com/32043036/183223635-ea351f8f-a5a4-4639-a94e-8b92a042f2bb.png"> 
   <p align="left"> <br>
6. Using filters, sort the percent change column Z-A to see the greatest percent changes on top.
     <p align="center">
<img width="277" alt="sort-percent-change" src="https://user-images.githubusercontent.com/32043036/183223798-bfb1787d-052c-4c3c-a554-8897c98bd9fb.png">
<p align="left"> <br>

  
  #### *The School of Information Management saw the greatest percent increase in instructional funding at +241%. The only college with less funding in 2019-2020 than in 2015-2016 was the School of Public Health.*
  
  
  <p align="center">
  <img width="1045" alt="final-percent-change" src="https://user-images.githubusercontent.com/32043036/183224149-5a0dd9ea-bf71-46d2-9819-a68364a58867.png">

  
### Did any departments or colleges have less funding in 2020 than in 2015?

### Which major in the College of Engineering had the most instructional funding per undergraduate student in 2019-2020?
  1. Find the breakdown of undergraduate enrollment using the Wayback Machine for the [College of Engineering Facts and Figures page](https://engineering.berkeley.edu/about/facts-and-figures/). Enter the data into a new column in the datasheet. 
    <p align="center">
      <img width="1118" alt="Screenshot of the Wayback Machine showing the capture for the College of Engineering numbers in Februrary 2021." src="https://user-images.githubusercontent.com/32043036/183275514-bf1abd41-88ce-471c-9f0b-5570b490dfae.png">
<p align="left"> <br>
  2. In a new column, calculate instructional dollars per student using a formula.
  <p align="center">
    <img width="619" alt="Screenshot of column with funding per student formula: divide the cell with the 2019-2020 instructional funding by the cell with 2019-2020 undergraduate enrollment." src="https://user-images.githubusercontent.com/32043036/183275530-41fb82d8-98f9-418f-ab73-5c24538965f4.png">
<p align="left">
  
#### *Industrial Engineering and Operations Research had the most instructional funding per undergrad at $44.*
  
### Which three departments within the College of Letters and Science had the most funding for each year?
  
  strategic planning for CoE 
  PIs?
  how has the curriculum changed? (MSE 45 lab)
  how have the courses changed - course offering? 
  # of units in each department correlated with $$ 
  
  
