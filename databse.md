No Sequal Databases:

Advantages:
1) Data is stored as JSon with column names as the key. All the relevant data is stored in one blob so insertions and retrievals are fast as we can do awya without joins. 
2) If new columns are needed to be added for new data and we don't care about old data, NoSequal is better since we can staright away start adding new data without touching old data. In sql we have to add a new column and provide values for laready stored data which is expensive. 
3) Better horizontal partitioning. 
4) Better for aggregation and analytics. Thats why companies use nosql for analytics.

Disadvantages:
1)If there are a lot of updates, it becomes costly.
2) Consistency is a problem - acid is not guranteed. therefore financial institutions don't use nosal  for transactions
3)Are not read optimized. Takes a long time if you have to read many values
4)Relations are not implicit. You can't enforce a foreign key contraint
5) Joins are hard 





MongoDB

SQL              Mongo
Table            Collection
Row              Document
Column           Field

Collection isn't strict about what goes in it.
