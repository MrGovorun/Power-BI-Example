# Example of Power BI report
   This is example of Power BI report with data from open source https://trudvsem.ru/opendata/datasets (n.11) "Вакансии Приволжского федерального округа из ЕЦП «Работа в России»". Dataset contain data about open vacancies in some regions in Russia at 29.10.2022  
   
   I creat pretty background with gradient in online svg-generator and use it in report. Report containt three pages - two with data and one with map. Dataset containt information about min and max salary, but every row can include only min salary, both value or emtpy values in both columns. I check average of minimal and maximal salary separatly, but in some slice max salary can be lower than min salary, because max salary more often empty. I decide create new dimension, that contain difference between max and min values (min if only min exist and 0 if both empty). Than I filtered null-values and calculate average salary. It seems more correct decision  
   
   I also ranked count vacancies by sphere and print only top 5 spheres per region on first page of report. 
 
 __List of steps__:  
 1. Prepare data (remove some columns, change data type)
 2. Add schemas (create table with russian dayname and company size for mapping)
 3. Create dimensions and measures for correct presentation
 4. Make pretty backgrounds and forms
 5. Add filters for interactivity
 

