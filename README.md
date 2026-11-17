# Student Lifestyle, Study Habits, and Well-Being Analysis (Tableau Dashboard)

![Dashboard Preview](dashboard_preview.png)

## Project Overview
This interactive **Tableau** project analyzes the relationship between **Student Count (SC)** and key academic, lifestyle, and well-being indicators across a dataset of **502 student records**. The dashboard examines how sleep duration, daily study hours, study satisfaction, academic pressure, and financial stress are distributed throughout the student population.

---

## Objectives
* **Standardize Raw Survey Data:** Transform raw numerical and text-based survey responses into structured analytical tiers for clearer reporting.
* **Identify Behavioral Patterns:** Evaluate student distribution across daily study hours and sleep habits.
* **Assess Well-Being and Stress Factors:** Compare academic pressure, financial stress, and study satisfaction across standardized 1–5 rating scales.

---

## Dashboard Breakdown and Key Findings

### 1. Sleep Duration (SD) and Student Count (SC)
* **Grouping Logic:** Raw sleep responses were categorized into four qualitative tiers:
  * **Less than 5 hours:** `NOT GOOD` (123 students)
  * **5–6 hours:** `MODERATE` (123 students)
  * **7–8 hours:** `GOOD` (128 students)
  * **More than 8 hours:** `BEST` (128 students)
* **Key Finding:** The sample is evenly balanced between students achieving optimal sleep (`GOOD` and `BEST` = 256 students) and those experiencing insufficient or moderate sleep (`NOT GOOD` and `MODERATE` = 246 students).

### 2. Study Hours (SH) and Student Count (SC)
* **Visualization:** Area chart tracking student volume across daily study hour increments (ranging from 29 to 53 students per interval).
* **Key Finding:** Student distribution peaks at **53 students** in the upper-middle study range before tapering slightly at the highest end (**46 students**).

### 3. Study Satisfaction (SS) and Student Count (SC)
* **Scale:** 1 (Lowest Satisfaction) to 5 (Highest Satisfaction).
* **Distribution:**
  * **SS-1:** 86 students
  * **SS-2:** 100 students
  * **SS-3:** 103 students
  * **SS-4:** 116 students *(Highest cohort)*
  * **SS-5:** 97 students
* **Key Finding:** Overall satisfaction skews positive, with **SS-4** representing the largest single group (**116 students**).

### 4. Academic Pressure (AP) and Student Count (SC)
* **Scale:** 1 (Lowest Pressure) to 5 (Highest Pressure), ranked by student volume.
* **Distribution:** **AP-3** (125) > **AP-1** (99) > **AP-5** (98) > **AP-4** (92) > **AP-2** (88).
* **Key Finding:** Moderate academic pressure (**AP-3**) is the most prevalent category, accounting for nearly **25%** of all respondents.

### 5. Financial Stress (FS) and Student Count (SC)
* **Scale:** 1 (Lowest Stress) to 5 (Highest Stress), ranked by student volume.
* **Distribution:** **FS-1** (110) > **FS-2** (102) > **FS-3** (100) > **FS-5** (96) > **FS-4** (94).
* **Key Finding:** Student counts decline steadily as financial stress increases, with **FS-1** (lowest stress) representing the largest group (**110 students**).

---

## Tools and Methodology
* **Data Preparation and Feature Engineering (Excel / Google Sheets):**
  * Standardized text-based sleep durations into qualitative performance tiers (`NOT GOOD`, `MODERATE`, `GOOD`, `BEST`) using `IFS` logic.
  * Classified continuous numerical metrics into structured analytical bins for aggregation.
* **Data Visualization (Tableau):**
  * Designed a five-panel executive summary dashboard incorporating circle plots, area charts, bar charts, and shape-encoded distributions.
  * Implemented consistent metric abbreviations (`SC`, `SD`, `SH`, `SS`, `AP`, `FS`) across views for rapid cross-chart comparison.

---

## Repository Structure
```text
├── README.md                 # Project documentation and analytical findings
├── dashboard_preview.png     # Static image preview of the Tableau dashboard
├── data/                     # Cleaned dataset (.xlsx / .csv)
└── tableau/                  # Packaged Tableau Workbook (.twbx)
```

---

## How to View and Use
1. **Interactive Web Version:** Open the **Tableau Public** link at the top of this document to explore the dashboard in a web browser.
2. **Local Workbook:** Download the `.twbx` file from the `tableau/` directory and open it using **Tableau Desktop** or **Tableau Reader**.

---


