# Project 2 Analysis  

## Introduction  
As a former job seeker, I've always been suprised by the lack of data exploring the most optimal jobs and skills in the data science market. I  
set out to understand what skills top employers request and how to land better salaries.  

## Questions To Analyze  

To understand the data science job market, I asked the following:  
  1. Do more skills equal better pay?
  2. What are the salaries for data jobs in different regions?
  3. What are the top skills of data professionals?
  4. What skills demand the top salaries?

## Excel Skills Used  

The following Excel skills were utilized for this analysis:  
📊 Pivot Tables  
📈 Pivot Charts  
🧮 DAX (Data Analysis Expressions)  
🔍 Power Query  
💪 Power Pivot  

## Data Jobs Dataset  
The dataset used for this project contains real-world data science job information for 2024.  

## 🔍 Skill: Power Query (ETL)  
### 📤 Extract  
  * I first used Power Query to extract the original data and create two queries:
    - 🗂️ First on with all the data jobs information.
    - 🔧 The second listing the skillsfor each job ID.

### 🔄 Transform  
  * Then I transformed each query by changing column types, removing unnecessary columns, cleaning text to eliminate specific words,
    and trimming excess white space.

    - 📊 data_jobs_all
      
    ![PQ_data_jobs_salary](https://github.com/user-attachments/assets/270df7df-0a39-4965-b28c-98b3f1d24218)

    -🔧 data_job_skills

    ![PQ_ data_jobs_skills](https://github.com/user-attachments/assets/b2f671f1-def7-42a8-82a4-57511af1200b)

### ♾️Load  
* Finally, I loaded both transformed queries into the workbook, setting the foundation for subsequent analysis.

  - 📊 data_jobs_all
    
    ![PQ_WB_data_jobs_salary](https://github.com/user-attachments/assets/4f45210f-7ae9-478a-a88f-13c9e4b3c77c)

  - 🔧 data_job_skills
 
    ![PQ_WB_data_jobs_skills](https://github.com/user-attachments/assets/372d0642-267e-416a-8e5b-b08a149d175e)

## 📊 Analysis  

### 💡Insights  
  * 📈 There is a positive correlation between the number of skills requested in job postings and the median salary, particularly in roles like
       Senior Data Engineer and Data Scientist.
    
  * 💼 Roles that require fewer skills, like Business Analyst, tend to offer lower salaries, suggesting that more specialized skill sets
        commandhigher market value.
    
    ![Skills vs Money](https://github.com/user-attachments/assets/ab396a86-ae55-4d1e-8d0c-603dd6ad6d25)
