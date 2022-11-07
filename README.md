# Example of Power BI report
   This is example of Power BI report with data from open source https://trudvsem.ru/opendata/datasets (n.11) "Вакансии Приволжского федерального округа из ЕЦП «Работа в России»". Dataset contains data about open vacancies in some regions of Russia on 29.10.2022  
   
   I created pretty background with gradient at online svg-generator and used it in this report. It contains three pages - 2 data pages and 1 map. Dataset contains information about min and max salary, but every row can include only min salary, both value or emtpy values in both columns. I checked apart average minimum and maximum salary, but because of partly empty cell "max salary" in some sections the average maximum can be less than the average minimum. I decided to create new dimension, which contains the difference between max and min values (min- if only min exist and 0- if both empty). Than I filtered null-values and calculated the average salary. It seems to me this decision is more correct.  
   
   I also ranked number of vacancies by sphere and displayed only Top-5 spheres per region on the first page of report. 
 
 __List of steps__:  
 1. Prepare data (remove some columns, change data types)
 2. Add schemes (create table with days of the week in russian language and company size for mapping)
 3. Create dimensions and measures for correct presentation
 4. Make pretty backgrounds and forms
 5. Add filters for interactivity
 

