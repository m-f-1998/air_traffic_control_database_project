# Air Traffic Control Database Project

### Created by Matthew Frankland (April 2018)
### Source Material Locked Due to Similarities with Current Coursework. Email mf48@hw.ac.uk to Request Password.

## Problem Specification

T1 - Database System Aim - “Watt Airlines needs to manage their flights, crews, and passengers.”
Extend the above database system aim to be a detailed system requirement from which you can design a database schema. You need to extend the scenario with more details as appropriate to fit the requirements of this database exercise – for example, take into account the features that you have to include in the ER diagram (see T2) and the type of SQL query that you are asked for. You are NOT asked to produce a complete set of requirements, fully working application, or a complete set of queries that the company would actually need to run your database system successfully. Rather, you are asked to use this scenario to demonstrate your proficiency in the various aspects of this assignment. You will need to extend the scenario quite a bit, and invent some extra details. Write a description of your extended scenario, so that the reader can understand how you come to the ER diagram in the next task. 

T2 - Conceptual Model - Design a database schema according database requirements you have identified in T1. 
Create an ER diagram for the conceptual model of your scenario. The diagram MUST include one-to-many and many-to-many relationships, ideally with a variety of participation constraints. It MUST also include several other advanced ER features such as: 
    • A recursive Relationship; 
    • Derived Attributes; 
    • Composite Attributes; 
    • Composite Keys; 
    • Repeating Attributes; 
    • Use of Generalization and Specialisation. 
This ER diagram should not show foreign keys, it should only show the relationships between entities, i.e. linking lines.  Each attribute only occurs ONCE in the diagram. Make a note of any details of the requirements that could not be captured by the diagram.

T3 - Translation into Relational Schema - Define a relational schema from your conceptual ER diagram and represent it as a data dictionary.
Use the steps given in the lectures to convert your conceptual design into a relational schema. The schema will include foreign keys, and extra tables where required, e.g. for many-to-many relationships. Primary and foreign keys should be clearly identified. Make a note explaining how it has been derived from the original conceptual ER diagram, for those cases where you have had to make a decision. Create a data dictionary for your tables – for each table, include column names, domain and other constraints (including keys).

T4 - Implementation of the Schema in MySQL - Generate a script to create the tables in MySQL using the innoDB storage engine. 
The data definition language statements must specify:
    • Appropriate types for the attributes
    • The primary key;
    • Constraints such as NOT NULL and UNIQUE whenever appropriate;
    • Default values if appropriate;
    • FOREIGN KEY constraints, together with the policy for reacting to changes
    • Write comments into the script explaining what is happening in each part.

T5 - Loading Data - Load interesting data into the database, experimenting with insert statements and the bulk loader.
The data should be realistic, and there should be enough to enable you to demonstrate a range of queries in T6. Write a report stating which data was loaded from insert statements, which from the bulk loader, plus the contents of a few sample related records from each table – this is to give the marker a feel for whether you have entered suitable data, without having to read insert statements or poorly formatted output from SELECT *.

T6 - Queries over the Database - You should provide queries for the following:
    • Three complex queries over the database, and
    • One transaction for your scenario containing multiple CRUD (Create, Read, Update, Delete) operations, e.g. you may look up a person, change some value, and then check the update has happened, or you may insert some new data that requires multiple tables to be updated.
Many queries are likely to contain search condition(s) in which the data is supplied at run-time.However, you should supply the query with data, e.g. WHERE gender='M'. A complex query is one that contains at least one of the following features:
    • Joins involving a composite key,
    • Joins involving the same table twice,
    • Aggregation with group by and having,
    • Nesting with aggregation,
    • Nested negation, involving NOT EXISTS or NOT IN
    • Using MySQL built in functions
    • Using views 
Don’t provide basic queries, since you will not get many marks for this.

T7 - Indexes - Index definition that is designed to speed up one of their queries. Write an SQL script containing a set of CREATE INDEX commands.

T8 - Java Application - For this part of the project you should extend the provided Java application to connect to your 
database. 
Download the Java application from Vision and refer to the separate document explaining the Java application. Alter the class JDBCMySQLApp to provide a selection of your own queries to run in the application. A sample set of queries is already there, and these should be altered or deleted. Instructions on what to  alter is in the code. There should be at least one query for each group member. Your queries could be a subset of the queries in T6, or some other suitable queries. Particularly, ensure that you include 
some prepared queries, updates of some kind, and some which are based on user input. It is more important that you demonstrate the range of types of Java coding rather than the range of SQL queries. Don’t forget to alter my comments if necessary. If allowing the user to type in data, do some form of validation.
