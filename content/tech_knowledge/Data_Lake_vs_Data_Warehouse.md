## Data Lake vs Data Warehouse

|Features|Data Lake|Data Warehouse|
| -------------- | ---- | --------- |
| data structure | raw  | processed |
| purpose | Not yet determined | For specific usage |
| User | Data scienctist | Business professionals |
| Accessibility | Highly accessible and quick to update | More complicateds and costly to make changes |

## Data Lake Structure

A data lake is a repository of information in its “raw” format, meaning the format in which it existed when it was first collected and added to the storage pool. 

- Establish [data governance](https://www.talend.com/resources/what-is-data-governance/). It helps to ensure that data can fulfill its intended purpose, and also helps to enable effective data quality and data security.
- Create [data catalog](https://www.talend.com/resources/what-is-data-catalog/). Its purpose is to make it easy for stakeholders within and outside your organization to understand the context of the data so that they can work with it quickly.
- Enable search.
- Ensure security. Data security may not always be essential for working with the data inside a data lake. But it is crucial for adhering to compliance requirements and ensuring that sensitive information remains private.

## Data Preparation

### Essential

- [Data quality](https://www.talend.com/resources/what-is-data-quality/) --> Prevent from bias resulting

### Features(works)

- Standardizing formats
- Enriching source data
- Remove outliers

### Steps

1. Gather data. Finding the right data.
2. Discover and assess data. Detecting patterns and outliers by visually navigating data or applying guided advanced analytics.
3. Cleanse and *validate(??)* data. Cleaning up the data is traditionally the most time consuming part of the data preparation process, but it’s crucial for **removing faulty data and filling in gaps**. Once data has been cleansed, it must be validated by testing for errors in the data preparation process up to this point. Often times, an error in the system will become apparent during this step and will need to be resolved before moving forward.
4. Transform and enrich data. Transforming data is the process of updating the format or value entries in order to reach a well-defined outcome, or to make the data more easily understood by a wider audience. Enriching data refers to adding and connecting data with other related information to provide deeper insights.
5. Store data. Once prepared, the data can be stored or channeled into a third party application—such as a business intelligence tool—clearing the way for processing and analysis to take place.

## Reference

- [Data Lake vs Data Warehouse](https://www.talend.com/resources/what-is-data-preparation/)
- [Data Preparation](https://www.talend.com/resources/what-is-data-preparation/)