# Portfolio
 
 _Written 2025-03-14_  &  _Updated 2025-11-10_
>Names/keys/tokens checked and redacted.

---

>2025-11: Python & ML Project (Ongoing)

---
2025-10  |  Advanced Analysis Group Project: "US Mass M*rder" (Python)
---

<details>
<summary>Read about the group project</summary>
<p>

This two week course introduced us to Data Science with Python: 
- Algorithms
- Standardization
- Encoding
- Train/test split
- Prediction

**Goal**
- Check data and find a red thread 
- Storytelling with data
- Presentation
  
**Plan**
- Individually test the data to then brainstorm as a group.
- Make a source dataset for the group to easily aggregate new data.
- Divide the work following our business case.
- Merge into a final product and work on our presentation script. 

**The story**

From Characteristics to Consequences
- Introduction (The Question): What measurable factors (about the offender, the location, the weapon) have the biggest influence on the human cost (number of victims killed) of an incident?
- Exploration (The Models): We will try to predict the number of victims killed. We'll start with a simple model and then use a more complex one to see what really matters.
- Conclusion (The Insight): The models reveal which factors are the most significant drivers of an incident's severity.

<details>
<summary>Takeaway</summary>
<p>
>Group project with new people can be a disaster even if the people are friendly and do try their best.

Really thought this group could manage something without me coordinating as I was busy with moving houses.
Issues were: 
- Bad communication
- Indecision
- Wrong LLM use
- Ignoring project plan
- No responsibility

I ended up doing everything except a brainstorming session, but luckily they somehow managed to say something 
during the presentation even if it was very broad and general info.

</p>
</details>

[[Project Notebook - GitHub (No repo)]](https://github.com/ARoos-BI24/MainPage/blob/main/images/MMGO.ipynb)


</p>
</details>

---
2025-09/10  |  Azure Projects: "Trial/Demo"
---

<details>
<summary>Read about the project</summary>
<p>

Learn to use Azure and some of its features. All work was indiviual while still being in a group to help each other.

**Lab1:**
- Cost management, budget, alerts
- SQL DB, Data Factory, DF Linked Services, DF Pipeline
- Logic Apps, IAM
  
**Lab2:**
- EventHub
- Logic App API POST, Tokens
- Databricks, CosmosDB
- Streaming EventHub to DataLake
- PowerBI integration

[[Lab1 PDF - GitHub]](https://github.com/ARoos-BI24/nbazuredocs/blob/main/Extra/DokLabb1.pdf)

[[Lab2 PDF - GitHub]](https://github.com/ARoos-BI24/nbazuredocs/blob/main/Extra/DokLabb2.pdf)

[[Notebooks - GitHub]](https://github.com/ARoos-BI24/nbazuredocs/tree/main/Notebooks)
 
</p>
</details>

---
2025-09 (2)  |  Statistics & Analysis Project: "Swedish macroanalysis" (PowerBI/Excel)
---

<details>
<summary>Read about the project</summary>
<p>

**Goal:** 
- Group presentation about Swedish macrodata using PowerBI dashboard.

**Plan:**
- To make it easier for the group I chose the subject that was left (Finance/OMXS20).
- Given data for "OMXS20" was missing date, a new source was found.  
- The data was aggregated (Year/Quarter/Month) so that the group can use it for their comparisons.
- My own comparisons needed standardized data and I used Excel to get a table with Z-scores.
- In PowerBI I chose to create a proper source file with fact/dim so the whole group can be on the same page.
- Final design is mostly me (except the logo) with groups approval.

**Takeaway:**
- Need to focus more on storytelling with data. 

--

<img src="https://github.com/ARoos-BI24/MainPage/blob/main/images/Screenshot%202025-11-10%20151907.png?raw=true" alt="image-1"/>
<img src="https://github.com/ARoos-BI24/MainPage/blob/main/images/Screenshot%202025-11-10%20151920.png?raw=true" alt="image-2"/>

</p>
</details>

---
2025-09 (1)  |  Statistics & Analysis Report: "EV growth & power requirement (2010-2023)"
---

<details>
<summary>Read the report</summary>
<p>

- Report is semi-written like a scientific paper to make it easier for the reader.

[[Project PDF - GDrive]](https://drive.google.com/file/d/1uWO6wdfZ20c7QIXQ5hNJ-sIGskOvY685/view?usp=sharing)

</p>
</details>

---
2025-05  |  ETL Projects: "Real world banking (SQL)" & "End-to-End ETL (Python)"
---

<details>
<summary>Read about the two projects</summary>
<p>

**OBS: Minimal documentation**
>Will improve documentation soon (2025-11-10)
- First project was mainly T-SQL in SSMS
- Second project was done in Python, but can also be completed in SSIS 

[[Project 1: Real world banking (SQL) - GitHub]](https://github.com/ARoos-BI24/SQLETL/blob/main/Project_1/ETL_Assignment_1.sql)

[[Project 2: End-to-End ETL (Python) - GitHub]](https://github.com/ARoos-BI24/SQLETL/tree/main/Project_2)

[[GitHub repo]](https://github.com/ARoos-BI24/SQLETL/)
- Repo has readme with project requirements

</p>
</details>

---
2025-04  |  Python Project: "Streamlit dashboard"
---

<details>
<summary>Read about the project and see images</summary>
<p>

>__As a BI-student my choice of data was simple: Business__

**Project requirement:** 
- "Du skapar sedan en enklare dashboard med streamlit, som utnyttjar visualiseringar från plotly".

I overdid it by redoing a PBI-project "HKV" from ground up in Python and visualize it with Streamlit. It was a good learning
experience to understand the pros and cons of these tools depending on the use case.

--

  <details>
  <summary>ETL Notes:</summary>
  <p>
   
   
Some Source files were only available on a server and module 'pyodbc' was needed to fetch them.

- Chose to save files as CSV so they are light weight. (Sales has almost 5 million of rows.)
- Run into the file size limit and fixed by truncating source file to max 50 MB for 'git push'. (Sales is now ~1.2 million rows.)
- Moved away from CSV to Excel trying to save datatypes.
- Run into a row-limit with Excel, also issues with preserving some datatypes with NaN and float, will try out 'Parquet'.
- 'Parquet' is working as expected, finally!

---

  </p>
  </details>

  <details>
  <summary>Calculation & Visualisation Notes:</summary>
  <p>
   
   
Goal will be to aggregate the following data and sort them into these dashboard pages with an additional Overview/Home page.

__Sales:__
- Margin_Pct
- Cost
- Revenue YTD, QTD, MTD, WTD
- Revenue per Department, Category, Product

__HR:__
- Employee calc by gender, birth_date, employement, salary
- Worked hours per month
- Tenure (Total time employed)
- SUM of OverTime Hours (Fixed Salary Only)
- SUM of OverTime Pay ()
- SUM of Hourly

__Promotion:__
- Revenue for a promotion
- Best and worst promotion
- Most earned and lowest performers
- Discount_Pct during promotion and the Cost of it

__Finance:__
- Expenses_Cost Sum and per Item (and as a negative) (Finance) Product_Cost (Variable_Costs)
- TB1 = Revenue_Sum + (- Cost)
- TB1_Pct = TB1 / Revenue_Sum
- Sum of Fixed_Costs
- TB2 = TB1 - Fixed_Costs
- Sum of HR_Costs = Salary + Pension + Employer_Cost + Vacation (account emp with termination)
- Earnings_Report = TB1 + Expenses_Cost_Sum + Fixed_Cost + HR_Cost
- Earnings_Report_Pct = Earnings_Report / Revenue_Sum

---

  </p>
  </details>

[[GitHub repo]](https://github.com/ARoos-BI24/py_streamlit_dashboard)

[[Project Notebooks - GitHub]](https://github.com/ARoos-BI24/py_streamlit_dashboard/tree/main/part_2/notebooks)
- part_2 is the main/final project
 

  <img src="https://github.com/ARoos-BI24/py_streamlit_dashboard/blob/main/part_2/notebooks/Screenshots/Screenshot%202025-11-10%20115729.jpg?raw=true" alt="image-1"/>
  <img src="https://github.com/ARoos-BI24/py_streamlit_dashboard/blob/main/part_2/notebooks/Screenshots/Screenshot%202025-11-10%20120204.jpg?raw=true" alt="image-2"/>
  <img src="https://github.com/ARoos-BI24/py_streamlit_dashboard/blob/main/part_2/notebooks/Screenshots/Screenshot%202025-11-10%20120437.jpg?raw=true" alt="image-3"/>
  <img src="https://github.com/ARoos-BI24/py_streamlit_dashboard/blob/main/part_2/notebooks/Screenshots/Screenshot%202025-11-10%20120701.jpg?raw=true" alt="image-4"/>
  <img src="https://github.com/ARoos-BI24/py_streamlit_dashboard/blob/main/part_2/notebooks/Screenshots/Screenshot%202025-11-10%20120855.jpg?raw=true" alt="image-5"/>

</p>
</details>

---
2025-03  |  Database Modelling Project: "Online Bank DB" (SQL)
---

  <details>
  <summary>Read about the project</summary>
  <p>

__Scroll all the way down in Gist for my comments and screenshots.__

[[GitHub Gist link]](https://gist.github.com/ARoos-BI24/1a32c19277843248011a7369635ca63e)

  </p>
  </details>

---
2025-02  |  Database Modelling Group Project: "eStore DB" (SQL)
---

  <details>
  <summary>Read about the project</summary>
  <p>

__Scroll all the way down in Gist for my comments about the project.__

[[GitHub Gist link]](https://gist.github.com/ARoos-BI24/ae770a5e605a565c6557f1be7f3a53c2)

  </p>
  </details>

---

>2024-12 to 2025-1: Leaving out SQL introduction

---
2024-11 | Data Visualisation Project: "US Candy Distrubutor" (PowerBI)
---

<details>
  <summary>Read about the project and see images</summary>
  <p>

__Designed by me for a team project presentation with a DarkMode toggle!__

--

Notes have some points missing as the presentation was split in two but sadly my teammate couldn't make it so I had 
to improvise, luckily I designed it and talking points was focused on design principles so it wasn't too hard.

It surprised me that all other teams focused mostly on the data in a Data Visualisation course!!

The setup was that after the presentation everyone would give a constructive feedback and I can happily report that
everyone was speechless, with only a question if there was a function to expand the scatterplot window dynamically to make it bigger. 
_Funny enough I thought about it but run out of time, so I'll keep that in mind and try making it in the future._

One issue that I pointed out at the end was the 'light pink'-buttons were completely 'white' on the presentation screen that was
caused by poor saturation, it never even crossed my mind that it could be an issue as I'm so used to having good colors with OLED screens.

Lesson learned, TN-panels is still a thing and not all screens have vivid colors in 2024/2025!

--

Good quote by our educator:
>"The right data, in the right format, to the right person in the right time – We are basically running an intelligence service here…"

--

<details>
  <summary>CLICK TO SHOW: Dashboard design images - LIGHT MODE</summary>
  <img src="https://github.com/user-attachments/assets/1a3816e6-5296-4cc1-bf6f-8d161d0645c8" alt="image-1"/>
  <img src="https://github.com/user-attachments/assets/387c1492-bce0-4133-9d80-e91ebe49fd64" alt="image-2"/>
  <img src="https://github.com/user-attachments/assets/44ed5d06-c563-484c-b17d-e7e83e1ae29d" alt="image-3"/>
  <img src="https://github.com/user-attachments/assets/8c164c35-2c3e-460f-a3fd-afcf3ca0ebfc" alt="image-4"/>
</details>
<details>
  <summary>CLICK TO SHOW: Dashboard design images - DARK MODE</summary>
  <img src="https://github.com/user-attachments/assets/66252dcc-823a-434d-8b19-6101275c794c" alt="image-5"/>
  <img src="https://github.com/user-attachments/assets/664e225c-12cc-493b-afce-b0e2fc23f96f" alt="image-6"/>
  <img src="https://github.com/user-attachments/assets/ff7fef09-8fc6-4a82-95e2-63be840a1a6b" alt="image-7"/>
  <img src="https://github.com/user-attachments/assets/645f24c7-1b79-40f0-b44d-2e87fb5fd7a6" alt="image-8"/>
</details>
<details>
  <summary> CLICK TO READ: Notes and keywords used in the presentation</summary>
  <p>

Operative
För operativ personal. Felsökning av data och skapande av rapportlistor.
- Logo_
"Denotation" klubba, "Konnotation" subjektiva innebörder.
- Navigation
Normans design principer:
- Synlighet, Feedback, Mappning, Begränsningar, Konsistens
Principer för UX design:
- Skala, Visuell hierarki, Balans, Kontrast 
Nielsens Heuristic:
(Mental genväg för att förenkla problem och undvika kognitiv överbelastning.)
- Synlighet, Konsekvent och standard, Förebygga fel

Knappar (Principles)
- Normans: Synlighet, Mappning, Konsistens
- UX design: Skala, Visuell hierarki, Balans, (Gestalt-principer)
- Nielsens: Flexibilitet och effektivitet, Aesthetic and minimalist design,
- Hjälp användare återställa, Hjälp och dokumentation.
 
Management
Spårar aggregerad data och förändringar. Avancerad analys för management.
- Nav: färg
- Total Revenue: linje diagram, stödlinjer
- Scatter plot: avancerad analys, korrelation, färger

Executive
Enkel visualisering (t.ex. linjediagram och nyckeltal).
- YTD
- Profit by Region
- Top 10 States

Overview: Översikt
Darkmode
</p>
</details>


[[Data source zipped - GDrive]](https://drive.google.com/file/d/1y8k1ub_aziTYxekMBtxGAPH7bGPP-R0f/view?usp=sharing)
- Might have been from Kaggle or similar website

[[PowerBI file - GDrive]](https://drive.google.com/file/d/1Sv_LPPmNaKLNJ-Y9SmFAx-1rNctE4Fki/view?usp=drive_link)
- Measures and tables were created by me and properly sorted in fact/dim etc.

</p>
</details>

---
2024-10 | PowerBI Group Project: "AirBnB" dashboard & presentation
---

<details>
  <summary>Read about the project and see images</summary>
  <p>

>__First Team project and foresahdowing of whats to come..__

--

This was a my first Team project but sadly only two out of four did the work. I focused on ETL, modelling and aggregating 
our business questions into data while also designing everything for the presentation.

Some (coding) challanges were:
- Data outlier country slicer and the normal country slicer are on the same page. (Not optimal)
- Comparison Data for diagrams were very challenging as I also coded the avregare comparison values, before I
  noticed that I could calculate the averages myself and then set that number as a comparison average value in
  diagrams. It wouldn't be dynamic but for a set period and one presentation it was more than enough and I at
  least could get 2-3 hours of sleep before the presentation.
- Map by Price and Map by Room wasnt used in the presentation but were complete (mostly? I think).
- That map plugin was really fighting me to show prices as it did the opposite of cardinality of diagrams, meaning
  when digrams were correct the map was wrong and vice-versa..

>_As a final note I accepted this challenge for learning purposes and do not accept this behavior in a professional setting!_

--

[[PowerBI file - GDrive]](https://drive.google.com/file/d/1HvHSNQD0Q0PPzbRoJEvqfliL2K4yPTRC/view?usp=sharing)
- Measures and tables were created by me and properly sorted in fact/dim etc.
- All got the same source files that were a bunch of csv files that I merged and sorted etc.

  <img src="https://github.com/user-attachments/assets/18176521-55af-4943-824f-a4e6d38cb1cc" alt="image-1"/>
  <img src="https://github.com/user-attachments/assets/37aabe2b-785f-4be8-97d4-4d1ae6988cbb" alt="image-2"/>
  <img src="https://github.com/user-attachments/assets/2289d9bd-f576-4051-a824-dc4b1b728e0e" alt="image-3"/>
  <img src="https://github.com/user-attachments/assets/620d3990-4963-4035-90f6-620506d42353" alt="image-4"/>


</p>
</details>

---
2024-09 | PowerBI Projects: First dashboard creations
--

<details>
  <summary>Read about the project and see images</summary>
  <p>
   
- Simple ETL with PBI Transform.
- Aggregating new data using DAX & mQuery.
- Images from first weeks and they are very themed.
- HKV (light one) was my first creation.

  <img src="https://github.com/user-attachments/assets/fa8734a4-e0e7-4209-a4ae-02cdbf340014" alt="image-1"/>
  <img src="https://github.com/user-attachments/assets/b699b61f-8553-434a-ac7d-0e8e8d46135f" alt="image-2"/>

</p>
</details>

---



