# Databricks Study Notes

This repository contains structured summaries and notes related to my studies on Databricks, a unified analytics and data processing platform built upon Apache Spark. It documents essential concepts, best practices, and practical applications of Databricks, alongside clarifications on key terminologies and workflows needed for effective use of the platform in data science and data engineering projects.

The main objective of this repository is to organize, verify, and consolidate my learning progress, ensuring that all information is accurate, clear, and comprehensive. Each section will be periodically reviewed and updated to maintain relevance and facilitate easy reference, supporting my professional development in the data field.

Fundamentals:

- In the 1980s business needed more than just relational databases, but a system to manage and process data.
- With that, Data Warehouse concept came to life, a platform with support to structured data to make BI and Analytics easier. But the problem is that it only had support for structured data, the schemas were inflexible, it struggled with volume and velocity upticks and had a long processing time.
- In the 2000s, a big data expansion happened, with the creation of Data Lakes, a new pratform capable of supporting not only structured data, but also semi or unstructured data, with streaming support and cot efficient in the cloud, support for AI and Machine Learning. But the problem with this platform was that it did not have transactional support, meaning that data couldn't be used by BI and Analytics straight away, and the flexible storage created problems like poor data reliability and data governance concerns, and it did not substitute Data Warehouses.
- When Data Lakes and Data Warehouses were used together, a lot of compatibility problems difficulted the integration, two different storages were needed and if data was used in BI it had to be transfered from the Data Lake to the Data Warehouse storage, meaning that there was some redundant data stored, besides that, the data governance processes needed to be different for each of those structures, and their uses were also limited to tasks that the structures were capable of doing.
- In this scenario, databricks was introduced to the world, the first and only Data Lakehouse in the cloud. Combining the best of Data Warehouses and Data Lakes.
- A unified foundation for all data, capable of Data Science & AI, ETL & Real-time analytics, Orchestration and Data warehousing.
- With a also unified data storage for reliability and sharing, unified security, governance and cataloging.
- With an open Data Lake, consisting of all raw data
- Key features:
  - Transaction Support
  - Schema enforcement and governance
  - BI support
  - Decouple storage from compute
  - Open storage formats
  - Support for diverse data types
  - Support for diverse workloads
  - End-to-end streaming
- Structured data:
  - Predefined format
  - Easy to query, share and analyze
  - Can be displayed in rows, columns and relational databases
  - Numbers, strings, dates
  - estimated 20% of enterprise
  - less storage needed
  - easier to manage
- Unstructured data:
  - No defined format
  - Messy and hard to search and analyze
  - Cannot be displayed in rows, columns and ralational databases
  - Audios, Images, Files, Videos, e-mails, spreadsheets
  - Estimated 80% of enterprise
  - More storage needed
  - difficult to manage
- Unstructured data is processed and transformed in semi or structured data most of the times, so it can be queried, analyzed or fed into models.
- Examples of Unstructured data transformed into structured data:
  - Text -> extract key info with NLP (Natural Language Processing) -> "I'm having a good day" -> columns: Text, Emotion
  - Images -> computer vision applied to detect features -> columns: file_name, contains person, contains text
  - Video -> Frame by frame analysis using computer vision or machine learning; Audio transcribed using Speech-to-text
- Raw unstructured data is a mess of puzzle pieces and structured data is the finished puzzle that you can interpret, query and analyze. 
