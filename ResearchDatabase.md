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

#### Premise
(Give a short rundown of what my application entails)

Because my application needs to show information, it also needs to store that information. Hereby is it essential that I store that information properly.
I have worked with SQL databases before, so I was inclined to set up a SQL database for this project. It came to my attention however, that a SQL database might not be the best (or most ideal) database type to use.The information I needed to store was very table like, so I didn't really know if a relational database was needed or necessary.

My objective will be to gather information about databases and have a basic understanding about different types of databases. I also want to know which database type suits which purpose and by extention know which one would suit my application.

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Types of databases
From the source we can gather that there are a lot of different types of databases, but the most used are: Hierarchical, Relational, Non-Relational and Object oriented databases.

#### SQL vs noSQL
NoSQL is an umbrella term for any alternative system to traditional SQL databases. Sometimes, when we say NoSQL management systems, we mean any database that doesn't use a relational model.
There are four kinds of this database: document databases, key-value stores, column-oriented databases, and graph databases.

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

------------------------------------------------------------------------------------------------------------------------------------------------------------------
### References
(Link all used references here. Use footnotes to reference sources)

[Types of databases](https://www.mongodb.com/databases/types)

------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Bonus
### Comparing AI generated answer to my research
#### My question
I give the AI my general idea of my website and my user stories and asked it to write me a research paper about which type of database would best suit my application. Keep in mind that I give it all my User Stories, including the ones I haven't finished / started. 
This means that the AI could give a different answer than I would need at the moment. 

My full question:

*"My application is a website for divers to get an overview of diving locations and fish. Has an interactive world map that shows diving locations that are clickable. When clicked show information about dive and fish at that location. Have a search function for both dives and fish. Dive listing shows information about that dive and which fish a diver would be able to see when taking that dive. Fish listing shows information about that fish and which diving locations a diver would be able to see that fish at.*

*Can you write a research paper about which type of database suits my application best?"*

My subsequent followup question:

*"My user stories:*
* *As a diver I want to see on a world map where diving locations are.*
* *As a diver I want to be able to click on a diving location to see wich fish are in that location.*
* *As a diver I want to know which diving locations I can see a specific fish at, because a diver wants to know where they could be able to see a certain fish.*
* *As a diver/user I want to be able to add information to the website, because this broadens the informaton on the website.*
* *As a admin I want to be able to see which users added which information, because than the admin can flag users spreading misinformation.*
* *As a admin I want to be able to ban users from editing information, because a user could add information that is nonsensicle.*
* *As a diver I want to be able to search for specific fish, because a diver wants to know more information about a fish.*
* *As a diver I want to see which fish I can see per dive.*
* *As a diver I want to be able to search for specific dives.*

*Can you use these to rewrite the research paper?"*

#### AI generated answer
The answer was the same for both questions in the sense that the AI wrote about the same types of databases for both.

The AI answer:

*"After reviewing your user stories, it is recommended to use a combination of databases to achieve the desired functionality of your application. The databases that can be useful for your application include:*

*Geospatial database: A geospatial database is designed to handle geographical data and would be useful for your world map that shows diving locations. It allows for the storage and retrieval of location-based data, making it useful for your interactive world map. Examples of geospatial databases include PostGIS, MongoDB, and Elasticsearch.
Relational database management system (RDBMS): An RDBMS is based on a table structure and allows for complex queries and relationships between tables. It would be useful for handling data that has many-to-many relationships, such as your fish and dive locations. Examples of RDBMS include MySQL, PostgreSQL, and Oracle.
Full-text search database: A full-text search database is optimized for searching large volumes of text-based data and would be useful for your search functionality. It allows for fast and efficient searches across multiple fields, including text, keywords, and metadata. Examples of full-text search databases include Elasticsearch, Solr, and Amazon CloudSearch.
Based on your user stories, the following databases can be used:*

*For the world map that shows diving locations, a geospatial database can be used to handle the location data for your diving spots.
For the search functionality, a full-text search database can be used to handle the search functionality.
For the relationship between dives and fish, an RDBMS can be used to handle the relationships between dives and fish.
To implement these databases, you will need to consider the following:*

*Data modeling: This involves designing the structure of your database, including tables, fields, and relationships. You will need to determine how to store your dive and fish data, as well as how to link them together.
Data indexing: This involves creating indexes on your data to improve search performance. You will need to determine which fields to index, as well as which type of indexing to use (e.g., full-text, geospatial).
API integration: This involves integrating your database with your web application using an API. You will need to determine which API to use, as well as how to securely connect to your database.
To address your user stories, the following can be implemented:*

*As a diver, you would be able to see diving locations on the world map. When you click on a diving location, you would be able to see which fish are at that location.
As a diver, you would be able to search for specific fish and see which diving locations you can see that fish at.
As a diver/user, you would be able to add information to the website, which would broaden the information on the website. This information would be stored in a database.
As an admin, you would be able to see which users added which information. This would allow you to flag users spreading misinformation.
As an admin, you would be able to ban users from editing information. This would prevent users from adding information that is nonsensical.
As a diver, you would be able to search for specific fish and see which dives you can see that fish at.
As a diver, you would be able to search for specific dives.
Overall, the combination of these databases will enable you to achieve the desired functionality of your application."*



#### Comparison
#### Final conclusion
