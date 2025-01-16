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

**📈 Pivot Table**  
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

**🤔 So What**  

   - Thesesalary insights are important for planning and salary negotiations, helping professionals and companies align their offers with 
     market standards while considering geographical variations.


# 3️⃣ What are the top skills of data professionals?  

## 🔧 Skill: Power Pivot  

**💪 Power Pivot**  
* 🔗 I created a data model by integrating the data_jobs_all_skills table into one model.
* 🧹 Since I had already cleaned the data using Power Query; Power Pivotcreated a relationship between these two tables.

**🔗 Data Model**  

* I created a relationship between my two tables using the job_id column.
  
 ![3_data_model](https://github.com/user-attachments/assets/92d66587-d6b8-4b5b-9a4a-32ec1a0bf96b)  

**📜Power Pivot Menu**  

* The Power Pivot menu was used to refine my data model and make it easy to create measures.

  ![3_power_pivot_menu](https://github.com/user-attachments/assets/bc51e1a2-03ac-46e6-bf64-f121622630e9)

## 📊 Analysis

### 💡Insights

* 💻 SQL & Python dominate as top skills in data-related jobs, reflecting their foundational role in data processing and analysis.
 
* ☁️ Emerging technologieslike AWS and Azure also show significant presence, underlining the industries shift twords cloud services and
   big data tecnologies.

  ![Top Skills](https://github.com/user-attachments/assets/1ae36176-2f92-4445-8a01-0b4c5455c667)

**🤔 So What**  

* Understanding prevelant skills in the industry not only helps professionals stay competitive but also guides training and educational
  programs to focus on the most impactful technologies.

# 4️⃣ What skills demand the top salaries?  

## 📊 Skill: Advanced Charts (Pivot Chart)  

**📈 Pivot Chart**  
* I created a combo Pivot Chart to plot median salary and skill likelihood (%) from my Pivot Table.
    - 🪙**Primary Axis:** Median Salary (as a Clusterd Column)
    - 👍**Secondary Axis:** Skill Likelihood (as a line with markers)
 
* To customize the chart, I added a axis title, removed the lines (skill likelihood), and changed the markers to diamonds.

## 📊 Analysis  

### 💡Insights  

* 💰 Higher median salaries are associated with skills like Python, Oracle, and SQL, suggesting their critical role in high-paying tech jobs.
  
* 📉 Skills like PowerPoint and Word have the lowest median salariesand likelihood, indicating less specialization and demand in high-salary
      sectors.
  
  ![4_skill_likelihood](https://github.com/user-attachments/assets/b2f171ce-6d1a-4cb1-9924-58ced2716b20)

**🤔 So What**  

* This chart highlights the importance of investing time in learning high-value skills like Python and SQL, which are evidently tied to higher
  paying roles, especially for those looking to maximize thier salary in the tech industry.

### Conclusion  

As a data enthusiast, I embarked on this Excel based project to uncover valuable insights about the data science job  
market. Using a dataset I've curated from real-world job postings, I analyzed job titles, salaries, locations, and essential skills. by leveraging Excel  
features like Power Query, Pivot Tables, DAX, and charts, I discovered key correlations between multiple skills and higher salaries, particularly in
Python, SQL, and cloud technologies. 
 

I hope this project serves as a practical guide for data professionals and provides an overview of the skills needed for higher-paying roles.
