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


 
