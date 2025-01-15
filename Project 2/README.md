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

# 1️⃣ Do more skills equal better pay?  

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

# 2️⃣ What are the salaries for data jobs in different regions?  

## 🧮 Skills: PivotTables & DAX  

📈 Pivot Table  
  - 🔢 I created a Pivot Table using the Data Model I created with Power Pivot.
  - 📊 I moved the job_title_short to the rows area and salary_year_avg into the values area.
  - 🧮 Then I added a new measure to calculate the median salary for jobs in the United States.

     ![DAX_median_us_job_salary](https://github.com/user-attachments/assets/f1d068fe-5fd2-4671-ae60-df102ae2537c)
  
  - 🧮 I used a similar measure to calculate median salary
    
     ![DAX_median_salary](https://github.com/user-attachments/assets/19268b2b-b872-47d0-921d-bb89f6239cb4)

## 📊 Analysis  

### 💡Insights  
  * 📝 Job roles like Senior Data Engineer and Data Scientist command higher median salaries both in the US and internationally,
        showcasing the global demand for high-level data expertise.

  * 💰 The salary desparitybetween US and Non-US roles is particularly noticable in high-tech jobs, which might be influenced by the
       concentration of tech industries in the US.
       
  ![Median_salary_non_US](https://github.com/user-attachments/assets/2547409f-91b0-4f20-bcbe-994d11d3e4f9)  

🤔 So What  

   - Thesesalary insights are important for planning and salary negotiations, helping professionals and companies align their offers with 
     market standards while considering geographical variations.


# 3️⃣ What are the top skills of data professionals?
