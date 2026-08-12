# Bootcamp_Universia
Bootcamp Universia - Primeiros Passos em Power BI

Criacao de um notebook na ferramenta Google LM

- Contexto e Objetivos: Notebook Learn Data Analytics, com o objetivo de aprender sobre Analise de Dados

- Curadoria de Fontes:
How to Learn SQL for Data Analysis - DataMites Offical Blog
Training Roadmap Data Analyst - Women4IT
What Is Databricks? Architecture, Use Cases, and How It Fits the Modern Data Stack
What is the medallion lakehouse architecture? | Databricks on AWS
Lecture 11 Data warehouse Schema - Gyan Sanchay
From ER Models to Dimensional Models Part II: Advanced Design Issues - Sonra
ETL vs ELT: Dive Deeper into Two Data Processing Approaches - Databricks
Aprenda as noções básicas do DAX no Power BI Desktop - Microsoft Learn
Data visualization best practices for Power BI reports - Tabular Editor
Statistics and Data Science - Washington University Bulletin

- Engenharia de Prompts e "Cicatrizes":
The provided sources offer a comprehensive guide to modern data analysis and engineering, focusing on the technical tools and conceptual frameworks necessary for effective business intelligence. They define DAX and SQL as foundational languages for managing databases and building complex calculations within Power BI Desktop, while also emphasizing the importance of user-centric visualization to ensure insights are clear and actionable. The documentation further compares ETL and ELT processing methods, explaining how the order of operations impacts data availability, scalability, and compliance within cloud-based architectures. Together, these materials highlight that quality reporting relies on a robust semantic model and a deep understanding of the business questions being addressed. Beginners are encouraged to master these technologies to solve real-world problems and drive efficient, data-driven decision-making.

The primary difference between ETL (Extract, Transform, Load) and ELT (Extract, Load, Transform) lies in the order of operations and where the data transformation occurs. While ETL has been the industry standard for decades, ELT is a newer approach that leverages the power of modern cloud storage and distributed processing.
Core Differences in Process and Architecture
Order of Operations: In an ETL model, data is extracted from sources, moved to a staging area for transformation into a usable format, and finally loaded into a storage repository for analysis. Conversely, ELT loads data into the repository immediately after extraction, and transformations are performed later, directly within the data repository as needed.
Infrastructure Requirements: ETL processes are often associated with traditional data warehouse architectures and can be run on physical, onsite servers. ELT is designed for modern data lake and lakehouse architectures, such as Databricks, which can store both structured and unstructured data (like logs or video files) in cloud-based environments.
Flexibility and Data Availability: ETL is a rigid, linear process; you must decide in advance how to transform and filter data, which limits the raw data available to downstream analysts. ELT is much more flexible because it stores raw, original data that can be transformed in multiple ways depending on the specific use case or new business requirements.
Performance and Scalability
Scalability: ETL is difficult to scale quickly because the upfront transformation stage is resource-intensive. ELT is highly scalable; because it runs on cloud-based platforms, organizations can load massive volumes of raw data without initial processing delays.
Speed: ELT offers faster initial loading times since transformation is deferred. However, ETL provides faster query performance once the data is loaded because it is already cleaned and formatted for immediate use.
Compliance and Storage
Data Governance and Compliance: ETL can be safer for highly regulated industries (like finance or healthcare) because sensitive information can be removed or masked before it is ever stored. With ELT, sensitive raw data is stored first, which requires careful management to remain compliant with regulations like HIPAA or GDPR.
Storage Needs: ETL typically requires less storage space because it only saves a selected subset of transformed data. ELT requires more storage because it retains the entire volume of raw data in various formats.
Modern Implementation: The Medallion Architecture
In modern analytics, these processes often manifest in a medallion lakehouse architecture, which organizes data into quality-based layers:
Bronze (Raw): Equivalent to the "Extract and Load" phase, where raw data is ingested in its original format.
Silver (Validated): The initial "Transformation" phase, where data is cleaned, deduplicated, and normalized.
Gold (Enriched): The final stage where data is highly aggregated and optimized for business intelligence and reporting.

- Miniguia de Estudo (Entrega Final): video "How DAX Filter Context Actually Works" e o Data Mindmap.

