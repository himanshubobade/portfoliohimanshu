---
title: "Work At JPL"
layout: "work-single"
draft: false

pageDescription: "Honored to have received a spot award at JPL’s 2023 product conference for my work in Data Engineering and Cloud Platform Engineering. This recognition highlighted the design and implementation of robust data pipelines, as well as the adoption of cutting-edge cloud technologies that enhance scalability and efficiency. I’m deeply grateful for the supportive and pioneering team I’ve had the privilege to collaborate with, and proud that our collective efforts continue to drive innovation in this exciting domain."
pageImage: "/images/jplAward.jpeg"

platforms:
  - platformHeading: "Use-Case Engineering"
    projectSectors:
      - sectorHeading: "A) Fibre"
        projects:
          - heading: "1] TAT Status"
            description: "Optimized Fibre Service Efficiency: Streamlined a 52-step tracking process by integrating real-time monitoring for technician service status. Engineered a data pipeline with Spark, Scala, Kafka, Airflow, APIs, Hive, and MySQL, ensuring seamless synchronization across 5 disparate systems with CI/CD testing. Enhanced service resolution efficiency, impacting 4.3 million users with real-time tracking and proactive alerts. "
            image: "/images/Fibre.png"
          - heading: "2] Live Device Theft Prevention"
            description: "Built a real-time Geofencing alert system to detect unauthorized device movement across geographical regions. Leveraged Spark, Hive, Kafka, Scala, and Airflow to process live location updates, reducing device theft incidents and enhancing security monitoring. "
            image: "/images/Theft.png"
          - heading: "3] Location-Based Customer Segmentation"
            description: "Developed a customer profiling solution by tracking day and night locations using public Kafka streams. Integrated NiFi, Kafka, Spark, Scala, Airflow, and Hive to process and analyze location data, enabling targeted premium service offerings based on user affordability and behavior insights. "            
            image: "/images/Location.png"


      - sectorHeading: "B) Migration Projects (HDP to CDP)"
        projects:
          - heading: "1] Network Tower Optimization, GIS, JPW, OrderCare, and WorkOrder"
            description: " Engineered scalable data pipelines for Network Tower Optimization, GIS, OrderCare, and WorkOrder, capturing KPIs to support enterprise-wide decision-making. Employed Spark, NiFi, Scala, Hive, MySQL, Kafka, and Airflow to aggregate and process critical mobility data. Additionally, directed migration efforts from HDP to CDP, ensuring seamless system transition and improved performance.Implemented metadata tracking and data lineage frameworks to boost data governance and compliance. "
            image: "/images/Migration.png"

  - platformHeading: "Platform Engineering"
    projectSectors:
      - sectorHeading: "A) Hybrid Pipeline"
        projects:
          - heading: "1] HDP to Azure Live Streaming with Flink"
            description: "Engineered a high-performance Apache Flink-based real-time data pipeline to bridge on-prem Hive and Oracle MySQL via Azure Synapse. Designed a 24x7 running Azure Notebook to process and sync Kafka-based data, achieving a peak processing capability of 500 million records daily. Executed robust checkpointing mechanisms to ensure fault tolerance and data integrity. "
            image: "/images/Hybrid.png"
      - sectorHeading: "B) Data Quality - GCP"
        projects:
          - heading: "1] GCP - Data Fusion"
            description: "Adopted two methods to capture DataFusion metrics. The primary approach involved running a Dataproc job that queries a CDAP endpoint to gather instance, namespace, project, pipeline, and job-level metrics. These metrics are then ingested into BigQuery and displayed in Looker Studio for real-time data ingestion monitoring. This setup flags anomalies quickly and streamlines root-cause analysis."
            image: "/images/Data Fusion.png"
          - heading: "2] GCP - Data Flow"
            description: "Relied on Cloud Monitoring Metrics to capture and segregate Data Flow metrics at the job ID level. Used SQL-like queries against these metrics, funneling them into Looker Studio for detailed visualization. This method ensures thorough oversight of each job’s data ingestion and processing behavior."
            image: "/images/DataFlow.png"
          - heading: "3] GCP - DataProc"
            description: "Addressed an Apache Spark metrics bug within Dataproc by crafting custom Spark Listeners. Packaged these listeners with each Dataproc job to collect key runtime metrics, which were then stored in BigQuery. Looker Studio dashboards provided a comprehensive view of these metrics, ensuring any irregularities were caught promptly."
            image: "/images/DataProc.png"
      - sectorHeading: "C) Data Quality - Azure Synapse"
        projects:
          - heading: "1] Azure Synapse - CopyActivity"
            description: "Established a metrics-logging framework for pipelines using Copy Activity. Logged pipeline metrics into SQL Pool, then performed Z-score–based anomaly detection. The final results were displayed in dashboards, enabling quick identification of unexpected trends in data loads."
            image: "/images/CopyActivity.png"
          - heading: "2] Azure Synapse - Data Flow"
            description: "Created a reusable DataFlow-based solution attachable to any production pipeline. It captures logs from various sources and sinks, then processes them in an Azure notebook. The processed data goes into SQL Pool, where Z-score analysis highlights anomalies, and visual dashboards present the outcomes."
            image: "/images/AzureDataFlow.png"
      - sectorHeading: "D) Data Quality - OnPrem"
        projects:
          - heading: "1] Kafka Metrics Monitoring"
            description: "Introduced a mechanism to verify data completeness between Kafka producers and consumers, ensuring no data leakage. Used shell scripts and HQL queries to calculate offsets in Kafka topics, storing them in HQL tables for monitoring. This approach quickly reveals ingestion discrepancies and safeguards data integrity."
            image: "/images/KafkaMetrics.png"
---




<!-- ---
layout: "work-single"
projects:
  - title: "Data Engineering at JPL"
    subtitle: "Building Scalable Pipelines"
    image: "/images/Hybrid Flink Pipeline.png"
    description: "Worked on NASA data ingestion pipelines..."

  - title: "Big Data Analytics"
    subtitle: "Cloud Infrastructure"
    image: "/images/Azure Pipeline.png"
    description: "Analyzed large datasets using Spark..."

  - title: "Machine Learning Projects"
    subtitle: "Predictive Modeling"
    image: "/images/GCP Pipeline.png"
    description: "Developed ML models for satellite imagery..."
--- -->