## What is Replatform?
- "Lift-and-shift" approach using the same Teradata engine in the cloud.Say for example using Teradata Vantage on Azure
## What is ReArchitect?
- Redesigning the entire workload using Azure-native services such as Azure Synapse, Data Factory, Databricks, etc. For example replace legacy Teradata procedures and logic with Azure-native components like
   - Azure Synapse,T-SQL,ADF (Azure Data Factory),Apache Spark,Databricks
## Which Approach to Choose?(Motivation Factor)
- ### Replatform
  -   Organizations have immediate cluster expansion or renewal pressures. But the client has made significant investments in Teradata
  -   Desire to maintain hybrid/multi-cloud architecture
  -   Data explosion and need to leverage elasticity of compute cloud
- ### Rearchitect
    - Organizations have immediate cluster expansion or renewal pressures.
    - Complete Re-engineering to Cloud native solutions to eliminate current system gaps and move to future ready cloud warehousing solution.
    - In Preparation for Streaming work loads and, Delta Lakes and very high volume of transactions.
## Pros & Cons of each approach
- ### Replatform
  - Retains Teradata appliance (hybrid architecture)
  - Low Code Change,as we can reuse existing  *Terradata* objects like Stored Procedure, BTEQ scripts, so the migration is less complex.
  - Cons :
        - Limited or Pre-defined scaling.
- ### Rearchitect
- Auto-scaling for dynamic workloads.On Demand or Provisioned Resources
- Cost offering: Pay-as-you-go model and Provisioned resources for predictable workloads
- Cons:
   - Migration is complex, includes high code changes.
      ![Why it is complex](https://github.com/ZosBHAI/pure_theory/blob/main/terradata_to_synapse_migration_phases.png)
   - ## Following are steps in migrating
    - Schema and Object Migration
      1) Data Type Mapping - Ensuring accurate conversion of data types (e.g., DECIMAL, VARCHAR, DATE) to their Synapse equivalents to prevent data loss or corruption.
      2) Indexing Strategies - Translating Teradata's primary indexes and secondary indexes to Synapse's clustered columnstore indexes, heaps, and clustered indexes for optimal performance.
      3) Partitioning Schemes - Adapting Teradata's partitioning methods to Synapse's distributed table designs, including hash and round-robin distributions.
    - Historical Data Migration and Ongoing Data sync
       1)  Parallel data loading techniques.
       2)  Data validation and reconciliation.
       3)  Incremental load strategies for ongoing data synchronization.
       4)  Performance tuning for large datasets.
    - Rewriting the Workload for Cloud
      1) Azure Data Factory (ADF): For orchestrating data movement and transformations.
      2) Apache Spark: Leveraging its capabilities for large-scale data processing within Azure Synapse Spark pools or Azure Databricks.
         
  


 
