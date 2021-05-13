# Data Lake Structure

## Data Lake features

- 数据接入: 
  1. Store data
  2. Create meta info for the data file
  3. Provide a method to access the data. For instance, API or port(?).
- Data storage
- Data search 
- Data management:
  1. Create meta info
  2. Create *tag of data*(?) and classify the data. Create *data index*(?)
  3. Create relation between different types of data
  4. *Track the timeline of data*(?)
- Data quality
  1. Validate the completeness of data
  2. Monitor the data process procedure --> Apache Airflow / Zabbix
- Safety monitor: Monitor the usage of data, knowing the user and usage(what operation has been done), and hide sensitive info in data.
- The easy use of explore data: Basic tools or methods for other users to explore the data.

## Layering

1. **Raw** data layer - also called the **Ingestion/Landing area** because it's literally the sink of our data lake. The main objective is to ingest data into **Raw** as quickly and as efficiently as possible. **Raw** still needs to be organized into folders. It may be good to start with generic division: `subject area/data source/object/year/month/day` of raw data.
2. **Standardized** data layer - may be considered as optional in most implementations. The main objective of this layer is to improve performance in *data transfer* from **Raw** to *Curated*(?). In **Raw**, data is stored in its *native* format, in **Standardized** we choose the format that fits best for **cleansing**. The structure is the same as in the previous layer but it may be partitioned to lower grain if needed.
3. **Cleansed** data layer - also called Curated Layer/Conformed Layer. Data is transformed into consumable data sets and it may be stored in files or tables. The purpose of the data, as well as its structure at this stage is already known. In regards to organizing your data, the structure is quite *simple and straightforward*. For example: `Purpose/Type/Files`. Usually, end users are granted access only to this layer.
4. **Application** data layer – also called the Trusted Layer/Secure Layer/Production Layer, sourced from Cleansed and enforced with any needed business logic.
5. **Sandbox** data layer – another layer that might be considered optional, is meant for advanced analysts’ and data scientists’ work. 

## Important components in data lake structure

- Security
- Governance
- Metadata
- Stewardship
- Master data
- Archive
- Offload
- Orchestration + ETL processed

## Other important aspects

A well-planned approach of designing these areas is essential to any Data Lake implementation. We need to think of the desired structure we would like to work with. On the other hand, being too strict in these areas will cause Data Desert (opposite to Data Swamp). The Data Lake itself should be more about empowering people, rather than overregulating. 

Most of the above problems may be solved by planning the desired structure inside your Data Lake Layers and by putting reliable owners in charge. From our experience, we see that the organization of Data Lakes can be influenced by:

- Time partritioning
- Data load patterns(real-time, streaming, incremental, full load, one time)
- Subject areas/source
- Security boundaries
- Downstream app/purpose/uses
- Owner/stewardship
- Retention policies
- Business impact
- Confidential classfication

## The achievement should be reached by Data Lake

- 3 v's(**velocity**, variety, volume). We may operate on a variety of data, high in volume, with incredible velocity. The important fact is that **velocity** stands here not only for the processing time, but also for time to value, since it’s *easier to build prototypes and explore data*.
- Reduced effort to ingest data(**Raw** Layer), deplay work to plan the schema and create models until the value of the data is known
- Facilitate advanced analytics scenarios.
- Storage large volumes of data cost efficiently. There is no need to think if the data will be used, it can be stored just-in-case. Properly governed and managed data can be collected till the day we realize that it might be useful.

-------------

### REF

- [Data lake structure](https://lingarogroup.com/blog/data-lake-architecture/)