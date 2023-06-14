# Research
------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Introduction
(Give a short rundown of why I ask the question)

I am writing this research paper because I want to know which type of database suits my application best.
My application is a website for divers to get an overview of diving locations and fish. Have an interactive world map that shows diving locations that are clickable. When clicked show information about dive and fish at that location. Have a search function for both dives and fish. Dive listing shows information about that dive and which fish a diver would be able to see when taking that dive. Fish listing shows information about that fish and which diving locations a diver would be able to see that fish at.

#### methods
(What methods do I use to research this topic?)

There are a lot of different methods for researching. 
The main ones are: 
* Observation / Participant Observation
* Surveys
* Interviews
* Focus Groups
* Experiments
* Secondary Data Analysis / Archival Study
* Mixed Methods (combination of some of the above)

Of these methods I will mainly use Secondary Data Analysis / Archival Study, but I would also like to gather information through other people.

#### execution
(How did I execute this method and research?)

I searched on internet and our school courses for information. 
I also discussed this topic with a teacher and gathered information through that. 

#### Premise
(Give a short rundown of what my application entails)

Because my application needs to show information, it also needs to store that information. Hereby is it essential that I store that information properly.
I have worked with SQL databases before, so I was inclined to set up a SQL database for this project. It came to my attention however, that a SQL database might not be the best (or most ideal) database type to use.The information I needed to store was very table like, so I didn't really know if a relational database was needed or necessary.

My objective will be to gather information about databases and have a basic understanding about different types of databases. I also want to know which database type suits which purpose and by extention know which one would suit my application.

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Types of databases
From the source we can gather that there are a lot of different types of databases, but the most used are: Hierarchical, Relational, Non-Relational and Object oriented databases.[^1]
But these all fall under two terms: SQL or noSQL.

#### SQL vs noSQL
NoSQL is an umbrella term for any alternative system to traditional SQL databases. Sometimes, when we say noSQL management systems, we mean any database that doesn't use a relational model.
There are four kinds of this database: document databases, key-value stores, column-oriented databases, and graph databases.

SQL databases are built upon relations between tables. You therefore use SQL databases when you need two tables to relate to eachother. For example; when you are writing user stories and you notice that two (or more) entities need to have a relation to each other. 
NoSQL databases are used when no relations are needed. This can be the case if you need to store simple data (like accounting data or an Exel sheet).
(When do you use an SQL or noSQL database?)

#### Most popular databases 
The hierarchical database is like a family tree and offers high performance, as there’s easy access and a quick querying time.
The relational database stores data in discrete tables.
The non-relational database matured due to increasingly complex modern web applications.
The object oriented databases are unique because associations between objects can persist. This means that object oriented programming and the querying of data across complex relationships is fast and powerful.

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### results
(What are the results of this research?)

### Conclusion
(What is the  conclusion of this research?) 

Because my application needs to have a relation between dives and fish(es), that means I have to 

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### References
(Link all used references here. Use footnotes to reference sources)

[^1]: [Types of databases](https://www.mongodb.com/databases/types)

------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Bonus
### Comparing AI generated answer to my research
#### My question
I give the AI my general idea of my website and my user stories and asked it to write me a research paper about which type of database would best suit my application. Keep in mind that I give it all my User Stories, including the ones I haven't finished / started. 
This means that the AI could give a different answer than I would need at the moment. 

My full question:

*"My application is a website for divers to get an overview of diving locations and fish. Has an interactive world map that shows diving locations that are clickable. When clicked show information about dive and fish at that location. Have a search function for both dives and fish. Dive listing shows information about that dive and which fish a diver would be able to see when taking that dive. Fish listing shows information about that fish and which diving locations a diver would be able to see that fish at.*

*My user stories:*

* *As a diver I want to see on a world map where diving locations are.*
* *As a diver I want to be able to click on a diving location to see wich fish are in that location.*
* *As a diver I want to know which diving locations I can see a specific fish at, because a diver wants to know where they could be able to see a certain fish.*
* *As a diver/user I want to be able to add information to the website, because this broadens the informaton on the website.*
* *As a admin I want to be able to see which users added which information, because than the admin can flag users spreading misinformation.*
* *As a admin I want to be able to ban users from editing information, because a user could add information that is nonsensicle.*
* *As a diver I want to be able to search for specific fish, because a diver wants to know more information about a fish.*
* *As a diver I want to see which fish I can see per dive.*
* *As a diver I want to be able to search for specific dives.*

*Can you write me a research paper about which type of database suits my application best?"*

#### AI generated answer
The AI answer:

*"To determine which type of database best suits your application, you first need to understand your application's requirements. Based on your user stories, it seems that your application needs to handle location data, search functionality, and user input. Here are some potential database options to consider:*

*Relational databases: These are the most common type of database and are good for handling structured data. They use tables with predefined columns and rows to store data. Relational databases are good for handling data that has a clear structure, such as user information or dive locations. They are also good for handling search functionality, as they can use SQL queries to quickly search through large amounts of data. Popular relational databases include MySQL and PostgreSQL.*

*NoSQL databases: These are non-relational databases that are good for handling unstructured data. NoSQL databases can be more flexible than relational databases, as they do not require predefined schemas. They are good for handling data that may have varying structures or that needs to be easily scalable. NoSQL databases can also be faster at handling large amounts of data. Popular NoSQL databases include MongoDB and Cassandra.* 

*Geographic databases: These are specialized databases that are designed to handle geographic data, such as location coordinates, maps, and spatial relationships. They are good for handling location data, such as dive sites and fish habitats. Geographic databases can also handle complex queries that involve spatial relationships, such as finding all dive sites within a certain distance of a given location. Popular geographic databases include PostGIS and MongoDB with GeoJSON.*

*Depending on the specific requirements of your application, one or more of these database options may be appropriate. It's also possible that a combination of different types of databases may be needed to handle different parts of your application. For example, you may use a relational database to handle user information and search functionality, while using a geographic database to handle location data.*

*When choosing a database, it's important to consider factors such as scalability, performance, and ease of use. You should also consider the specific features and capabilities of the database, such as its ability to handle complex queries or its support for geographic data.*

*Here are some resources to help you learn more about different types of databases and their use cases:*

[Relational Databases vs. NoSQL Databases](https://www.mongodb.com/nosql-explained/nosql-vs-sql) /
[What is a Geographic Database?](https://www.gislounge.com/what-is-a-geographic-database/) /
[PostGIS Documentation](https://postgis.net/documentation/) /
[MongoDB: How to Build a Geo-Enabled App](https://www.mongodb.com/how-to/geo-enabled-app)

*Ultimately, the choice of database will depend on the specific needs of your application and the trade-offs between different options. It may be helpful to prototype different parts of your application with different databases to see which works best in practice."*

#### Comparison
#### Final conclusion
