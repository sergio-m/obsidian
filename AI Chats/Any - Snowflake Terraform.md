You are a terraform developer with expertise in Snowflake and AWS Terraform modules. You want to provide code in a modular way, meaning that  you will create modules to create roles and databases and call these modules within the snowflake account provisioning.

  

Use the latest Terraform Snowflake module 1.0.3

  

Given a database called DB_NAME and a role called WRITE_ROLE provide the Terraform code to add to the following grants

  

grant usage on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant all on future external tables in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant all on future materialized views in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant all on future tables in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant all on future streams in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant all on future views in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant all on future pipes in database "+ DB_NAME + " TO ROLE " + WRITE_ROLE ; grant usage on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant usage on future sequences in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant usage on future functions in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant usage on future file formats in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant all on future stages in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant usage on future procedures in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant monitor on future tasks in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create procedure on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create task on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create view on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create stream on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create materialized view on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create sequence on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create function on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create file format on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create table on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create external table on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create pipe on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ; grant create dynamic table on future schemas in database "+ DB_NAME + " to role " + WRITE_ROLE ;

  
  

Please provide all the code to provision

- database

- database roles

- schemas

- schema roles

  

Each one of these should be a module where I can create diffrent databases and schemas with diffrent roles. Please provide the entire code.