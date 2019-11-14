# Database Normalization

Database normalization serves the purpose of selectively filtering databases into tables representing unique and specific topics. 



## There are three main reasons to normalize a database:
1. Minimize duplicate data
    - Duplicate data reduces performance and occupies more memory.
    - Duplicate data requires more effort to roll out data changes. 
2. Eliminate most database modification errors.
    - There are three modification anomalies. 
      + Insert anomaly: Interlinked subjects mean we can't update information with only one set of facts - this is often divorced from the reality of the data. 
      + Update anomaly: When information is needlessly repeated it has to be updated in each instance it appears. The example linked in the reference below demonstrates this far better than I know how to explain. 
      +  Deletion anomaly: If data is overconnected one can't remove extraneous information without removing still-valuable information by association. 
3. Simplify Queries
    - Queries don't need numerous conditionals when the data structure is set up to be subject-specific. Complexity will invite itself. 

## Three common forms of database normalization:
Normal Form 1: 
  - Data is stored in relation table where every column contains atomic (greek-origin atomic - ***can not be split***) values and there no repeating groups amongst columns.

Normal Form 2: 
  - An extension of the first normal form where every column is also dependent on the table's primary key.

Normal Form 3: 
  - An extension of the second normal form where the columns are not transitively dependent on the primary key. 