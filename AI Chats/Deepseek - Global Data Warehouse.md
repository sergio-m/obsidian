
Take on the person of a data architect with specialized knowledge in Snowflake, AWS and DBT. You work in a US health company which is under HIPAA , FDA and GDPR reugulations. Your goal is to come up with scalable data systems used for global reporting using Tableau in a way where none of the regulations are violated.

  

Current Environment:

We currently have 2 datawareshouses for the US and EU region. Both are hosted in AWS. Both warehouses contain PII and PHI data. This data is masked based on users roles. These roles decide if you have access to PII data or not. The individual warehouses collect data from various datasources like Salesforce, QAD, MySQL, Splunk. These datasources are not shared between regions. Each region has its own Salesforce, QAD, MySQL server and Splunk accounts.

  

The data from these datasources are ingested into their respective Snowflake account. This means that US Salesforce data flows into US Snowflake warehouse. The columns on each table have a PII tag that determins if the column contains PII data or not. Based on the user role, the PII data is rendered as-is or de-identified.

  
  

In Germany AWS region, we have a Global datawarehouse using Snowflake. This warehouse should ingest data from the US and EU warehouse and consolidate them to a schema using a specific topology. These tables will be used to build reports served globally using a Tableau site. All tables in the Global datawarehouse (GDW) have a country and region column to identify the source. The GDW has access roles based on country and region.

  

Requirements:

Design a solution that meet the specific requirements

- Use Snowflake replication technology and tagging

- non PII data needs to be replicated from US and EU to GDW using Snowflake technology

- scalable data grow

- Data Catalog and documentation to be updated automatically upon schema change

- Query auditing

- Report schema to map Tableau reports layout

- Snowflake only accessed via whitelisted IPs

- Be able to solve same tables in US and EU but with diffrent schemas. Ex. Some columns exists in US but not in EU schema

  
  

Nice to have:

- AI to assits on build queries using schema, catalog and documentation

- Api integration for external customer reports

  
  

Build me a solution that meets all the requirements and possible the nice to haves.