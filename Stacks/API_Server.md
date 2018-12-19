`API_Server`

The Server component needs to be shipped as a standalone API only server. 
The operational processing should be mostly like a MVC app which takes REST request , maps them through controller, may filter the input based on security and data validation , propagate to the business logic , implementing DAO and sending the data back .

The Idea is somewhat similar to how CMPS used to work. 
Not sure how modern the idea is , but i guess exploring a bit more would leverage more ideas or its valuability. 

Initially the Stack should include the following.

Runtime : Node. 
API framework : Express. 
Database : PostgreSQL + Mongo.(A polyglot seems nice at this place , but this would be much clearer when the database is designed).
ORM : For Postgre Sequelize seems a good option. Not sure about Mongo yet.
Presentation : Angular (this might definitely turn out to be extra heavy. This should be clearer during implementation).

Let's choose this much for a server stack just yet. We can think of a java Spring stack in a later milestone or maybe for a different App altogether.


    Stack Reference :[Mongo With Express](https://www.mongodb.com/blog/post/the-modern-application-stack-part-3-building-a-rest-api-using-expressjs) [Express & Postgre with sequalize] (https://scotch.io/tutorials/getting-started-with-node-express-and-postgres-using-sequelize)
