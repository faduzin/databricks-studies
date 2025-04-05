# Databricks Study Notes

This repository contains structured summaries and notes related to my studies on Databricks, a unified analytics and data processing platform built upon Apache Spark. It documents essential concepts, best practices, and practical applications of Databricks, alongside clarifications on key terminologies and workflows needed for effective use of the platform in data science and data engineering projects.

The main objective of this repository is to organize, verify, and consolidate my learning progress, ensuring that all information is accurate, clear, and comprehensive. Each section will be periodically reviewed and updated to maintain relevance and facilitate easy reference, supporting my professional development in the data field.

## Fundamentals of Databricks

### Historical Context:

- In the **1980s**, businesses required more than relational databases; they needed systems capable of managing and processing larger volumes of data efficiently.  
- This led to the development of the **Data Warehouse**, a platform designed specifically for structured data, enabling easier Business Intelligence (BI) and analytics. However, Data Warehouses had significant limitations:
  - **Inflexible schemas**
  - **Slow processing speeds**
  - Struggled to cope with increasing data **volume** and **velocity**
  - Supported only **structured data**

- In the **2000s**, the rise of **Big Data** gave birth to **Data Lakes**, platforms that could store not only structured but also semi-structured and unstructured data. Data Lakes offered:
  - Streaming data processing capabilities
  - Cost-efficient cloud storage
  - Support for AI and machine learning

  Yet, Data Lakes presented their own issues:
  - **Lack of transactional support**, making immediate use in BI and analytics challenging.
  - **Poor data reliability and governance**, due to flexible storage schemas and lack of enforced standards.
  - **Did not replace** Data Warehouses, but rather complemented them.

- Combining Data Lakes and Data Warehouses led to integration problems:
  - Different storage systems required data duplication and complex transfers between platforms.
  - Separate governance processes increased complexity.
  - Limited capabilities dependent on each structure's individual strengths and weaknesses.

---

### Emergence of Databricks and the Lakehouse Concept:

In response to these challenges, **Databricks** introduced the world’s first **Data Lakehouse** in the cloud, integrating the best aspects of Data Warehouses and Data Lakes into a unified solution.

- Databricks provides a unified foundation capable of:
  - **Data Science & AI**
  - **ETL and real-time analytics**
  - **Workflow orchestration**
  - **Data warehousing**

- Offers unified storage ensuring:
  - **Data reliability and sharing**
  - **Security, governance, and data cataloging**

- Utilizes an open Data Lake, enabling raw data storage and flexibility.

---

### Key Features of Databricks Lakehouse:

- **Transactional support** (ACID compliance)
- **Schema enforcement and governance**
- **Full BI support** and compatibility
- **Decoupling of storage from compute resources**
- Use of **open storage formats** (e.g., Delta Lake, Parquet)
- Supports **various data types** (structured, semi-structured, unstructured)
- Capable of handling **diverse workloads** (batch, streaming, machine learning)
- Provides **end-to-end streaming** capabilities

---

### Types of Data:

#### Structured Data:
- **Predefined formats** (rows and columns in relational databases)
- Easy to query, share, and analyze
- Examples: numeric data, strings, dates
- **Approximately 20%** of enterprise data
- Requires **less storage** and is **easier to manage**

#### Unstructured Data:
- **No predefined format**, messy, difficult to query or analyze directly
- Cannot be directly stored in relational databases
- Examples: audio, images, files, videos, emails, spreadsheets
- **Approximately 80%** of enterprise data
- Requires **more storage** and is **difficult to manage**

- Typically, unstructured data must first be processed and transformed into structured or semi-structured forms before meaningful analysis, querying, or use in machine learning models.

#### Examples of Transforming Unstructured into Structured Data:
- **Text** → Natural Language Processing (NLP)  
  Example:  
  - Input: `"I'm having a good day"`  
  - Output columns: `Text`, `Emotion`  

- **Images** → Computer Vision  
  Example:  
  - Output columns: `file_name`, `contains_person`, `contains_text`

- **Videos** → Frame-by-frame analysis using computer vision or machine learning; audio transcribed using speech-to-text.

---

### Analogy:

Raw unstructured data is like a box of puzzle pieces, chaotic and without clear meaning. Structured data is the completed puzzle, orderly and ready for interpretation, analysis, and querying.

