Welcome to your new dbt project!

### Using the starter project

Try running the following commands:
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](http://slack.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices


## Snowflake CI/CD POC

### Background

- Snowflake is increasingly being used for Transformation and Data warehousing. But it doesn’t offer any out-of-the
    box CICD solutions.
- Datalytyxis being evaluated for DataOps(CI/CD, Orchestration ) platform
- Extraction and Loading are done through Azure Data Factory and transformations are carried out in Snowflake via
    Streams, Tasks, and Stored Procedure

#### Problem

- Azure DevOps does not support the deployment of Snowflake native features (Tasks & Stored Procedures )
- Knowledge in JavaScript is required to write a stored procedure in snowflake
- Avoid rework if any DataOps tool is selected for Snowflake Projects

#### Solution

-Use DBT for Snowflake Development.

#### Benefits

- Able to perform continuous integration / Continuous delivery for Snowflake projects
- DBT Models are reusable and can be run against any Cloud data warehousing tool with minimal changes
- Business analysts and data scientists tend to speak in SQL and its much easier to collaborate
    with them.Anyone with SQL and basic knowledge of Python can easily develop a solution using DBT
- Data Lineage for Pipeline can be easily generated to understand which data sources are involved in a
    certain transformations and the flow of the data from source to target.
- All the computational work is pushed towards DW(Snowflake)
- Deploy Analytics code faster with software engineering best practices ( Environment, Package management
    and Continuous integration )
- DBT –a transformation tool is used to execute data transformations in Snowflake
- DBT is integrated with Azure DevOps & Snowflake Deployments are automated
- DBT -Models are created using the Jinja template which is executed in Snowflake

# Next Steps

## Enhance this Solution with Airflow for Data pipeline orchestration and Monitoring


