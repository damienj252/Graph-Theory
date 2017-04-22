# Graph-Theory
This is a project created in Neo4J based on a graph of the college GMIT and the relations between students, staff, times and rooms in the college

# Documentation:
There is a document attached to this repository explaining in detail the steps that were needed in order to complete this project. It took many attempts and many different angles but I have now completed a graph using Neo4J of my current Timetable of GMIT Galway.

# Requirements:
In order to complete this project I must first determine what is exactly needed in order to complete this project. I must determine the nodes, relationships, labels, relationship types and the properties of all the information I wish to add to the database. I have come to the conclusion that in order to complete this task effectively I must organise the details of what is needed in timetable in order for it to work effectively and efficiently. What I have discovered are described below:
Rooms
1.Student groups e.g. Third Year Software Development group A
2.Times e.g. Monday at 09:00 – 10:00 am
3.Lecturer e.g. Ian McLoughlin 
4.Subject e.g. Graph Theory

# Conclusion:
After completing this project I have realised that it is much more difficult than first expected. I made many different attempts in the order of the nodes and how to create the relationships that would be best suited to each node. I found that there was a lot of information that I had to put into the project and I had to be careful with the labelling of the nodes as there was many nodes that were needed to create this project. When I first began this project I didn’t realise that after creating a few nodes that the relationships would make it so hard to understand and the direction of each node was complicating at that time so I decided to create a small template to start with and then create my official project so there would be no mistakes but I still have some mistakes in my official project and I can’t seem to delete them without deleting all the relationships or node I have already created. If I were to do this project again I would take more time to distinguish the different type of nodes I would use but also I would try find a more direct way creating relationships between the nodes. I spent much of my time trying to fix the mistakes I created and this caused me to delete much of my project so in future attempts I would be more cautious on attempting a different project.
On another note I found this project to be quite enjoyable and I believe I have learned a lot after completing this project. I learned that in order to complete a successful project one must have a detailed outline of how they wish to complete such a large scale project. Each detail must be mentioned and sketches are a must in order to complete a project similar to this one.

# Queries: 
After completing this project I created some queries to test the graph created they are listed below:
These are the queries that work and gave me a return value.
MATCH(g:Groups) RETURN g.group
MATCH(d:Days) RETURN d.day
MATCH(t:Times) RETURN t.times
MATCH(l:Lecturs) RETURN l.name

This is a query I attempted but it would not return any values:
MATCH p=(l:Lecturs)-[r:Monday]->(s:Subject) WHERE s.name="Database Management" RETURN p




