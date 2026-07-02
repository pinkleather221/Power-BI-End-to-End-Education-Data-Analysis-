# End-to-End Power BI Analytics Project
### *Transforming Dirty Educational Data into Actionable Business Intelligence*

An **end-to-end Business Intelligence project** demonstrating how to transform messy educational data into meaningful insights using *PostgreSQL*, *Power Query*, *Power BI*, and *DAX*. This project covers the **complete analytics workflow** from securely connecting to a database and cleaning raw data, to designing a dimensional model, creating analytical measures, and building an interactive dashboard.


## Project Overview

Organizations rely on **clean, structured, and reliable data** to make informed decisions. However, operational data is often *messy, inconsistent, and stored in formats that are unsuitable for reporting*.

This project simulates a **real-world Business Intelligence workflow** using an education dataset containing information about:

- **Students**
- **Schools**
- **Teachers**
- **Academic Performance**
- **Subjects**
- **Geographic Locations**
- **Payments**

Rather than simply building charts, the project focused on the **complete BI lifecycle**:

- Connecting *securely* to a PostgreSQL database
- Cleaning and transforming data
- Normalizing a flat dataset
- Designing a **Star Schema**
- Creating relationships
- Writing reusable *DAX measures*
- Developing an interactive dashboard
- Generating meaningful business insights

---

## Project Objectives

The **primary objective** was to transform a *dirty operational dataset* into a reliable analytical model capable of answering key business questions.

The project focused on:

- Cleaning *inconsistent data*
- Removing **duplicates**
- Handling *missing values*
- Correcting *invalid data types*
- Designing a **dimensional model**
- Building relationships between tables
- Creating reusable **DAX measures**
- Developing an *interactive dashboard*
- Supporting **data-driven decision making**

---

## Dataset Description

The original dataset consisted of a **single flat table** containing information related to the education sector.

Some of the common *data quality issues* included:

- Missing values
- Duplicate records
- *Inconsistent spelling*
- Mixed uppercase/lowercase text
- *Incorrect data types*
- Invalid numerical values
- *Inconsistent location names*
- Repeated school information
- Repeated teacher information

These issues required **extensive cleaning** before analysis could begin.

---

## Technology Stack

| **Technology**      | **Purpose**                         |
|---------------------|-------------------------------------|
| *Power BI Desktop*  | Data Modeling & Visualization       |
| *PostgreSQL*        | Database Management                 |
| *Power Query*       | ETL & Data Cleaning                 |
| *DAX*               | Business Calculations               |
| *SQL*               | Data Retrieval                      |
| *Git & GitHub*      | Version Control                     |

---

## Project Architecture

```
PostgreSQL Database
        │
        ▼
Secure SSL Database Connection
        │
        ▼
Power BI Data Import
        │
        ▼
Power Query (Data Cleaning)
        │
        ▼
Star Schema Data Model
        │
        ▼
DAX Measures & KPIs
        │
        ▼
Interactive Power BI Dashboard
```

---

## Project Workflow

### 1. Data Extraction

The project began by connecting **Power BI** to a *PostgreSQL database* containing the educational dataset.

Unlike importing CSV files, this approach simulates a **production environment** where reports retrieve data directly from *enterprise databases*.

### 2. Secure Database Connection

To establish communication between Power BI and PostgreSQL, **SSL certificates** were configured to enable *encrypted data transfer*.

This step ensured **secure authentication** and protected data while in transit.

### 3. Data Cleaning *(Power Query)*

**Power Query** was used to transform the raw dataset into a *clean analytical dataset*.

Cleaning activities included:

- Removing *duplicate records*
- Replacing **missing values**
- Standardizing *location names*
- Correcting *spelling inconsistencies*
- Converting **data types**
- Formatting *date fields*
- Renaming columns
- Removing *invalid values*

All transformations were performed using Power Query's **Applied Steps**, making the *ETL process repeatable* during future refreshes.

---

## Data Modeling

The original dataset existed as **one large flat table**.

To improve *maintainability and analytical performance*, the dataset was normalized into a **Star Schema**.

### The Model Consisted Of

**Fact Table:**
- *Student Performance / Assessment Records*

**Dimension Tables:**
- *Student Dimension*
- *Teacher Dimension*
- *School Dimension*
- *Subject Dimension*

This approach **reduced redundancy** and simplified *DAX calculations*.

### Why Star Schema?

The **Star Schema** offers several advantages:

- *Improved report performance*
- **Reduced data redundancy**
- *Easier relationship management*
- **Simplified DAX calculations**
- *Better scalability*

### Relationships

Relationships were established using:

- **Primary Keys**
- *Foreign Keys*

Relationship types included:

- *One-to-Many*
- *Many-to-One*

**Single-direction filtering** was used where appropriate to improve performance and reduce ambiguity.

---

## DAX Measures

**Reusable DAX measures** were created to support analysis.

Examples include:

- *Total Students*
- *Total Schools*
- *Total Teachers*
- **Average Student Score**
- *Student Distribution*
- *School Distribution*

Concepts applied during development included:

- `SWITCH()`
- `IF()`
- `AND()`
- `OR()`
- `CALCULATE()`
- `FILTER()`

**Measures** were preferred over *calculated columns* whenever possible to ensure **dynamic calculations** based on report filters.

---

## Dashboard Design

The dashboard was designed to answer **key business questions** using *interactive visualizations*.

Visuals included:

- **KPI Cards**
- *Bar Charts*
- *Column Charts*
- *Donut Charts*
- **Tables**
- *Slicers*

Users can interactively filter reports by:

- *School*
- *County*
- *Region*
- *Teacher*
- *Subject*
- *Gender*

---

## Key Insights

The dashboard enables users to identify:

- **Student population** by school
- *Student distribution* across regions
- **Teacher allocation**
- *Gender distribution*
- **Academic performance trends**
- *Subject performance*
- **School performance**

---

## Challenges Encountered

During the project, several challenges were encountered, including:

### Dirty Data
The source dataset contained *inconsistent values* requiring **extensive cleaning** before analysis.

### Database Connectivity
Configuring **SSL certificates** was necessary to establish a *secure PostgreSQL connection* with Power BI.

### Data Modeling
Transforming a *flat table* into a scalable **Star Schema** required identifying *logical entities* and defining appropriate relationships.


---

## Getting Started

### Prerequisites

- **Power BI Desktop**
- *PostgreSQL*
- *PostgreSQL ODBC/Npgsql Driver* (if required)
- **SSL Certificate** *(for secure database connection)*

### Steps

1. **Clone this repository:**
   ```bash
   git clone https://github.com/pinkleather221/Power-BI-End-to-End-Education-Data-Analysis-.git
   ```
2. Open the `.pbix` file using **Power BI Desktop**
3. Update the *PostgreSQL connection details* if needed
4. **Refresh the data**
5. Explore the *interactive dashboard*

---

## Skills Demonstrated

This project demonstrates **practical experience** in:

- *Business Intelligence*
- **Data Cleaning**
- *ETL Development*
- **Power Query**
- *Data Modeling*
- **Star Schema Design**
- *SQL Databases*
- **PostgreSQL**
- *SSL Database Configuration*
- **DAX**
- *Dashboard Development*
- **Data Visualization**
- *Analytical Thinking*
- **Git & GitHub**

---

## Lessons Learned

This project reinforced that **successful Business Intelligence** is built on *strong data foundations*. While dashboards are the most visible outcome, the **real value** comes from ensuring data is *accurate, well-modeled, and capable of supporting reliable decision-making*.

Working through *secure database connectivity*, **data cleaning**, *dimensional modeling*, and **DAX development** provided practical experience that closely reflects **real-world BI projects**.