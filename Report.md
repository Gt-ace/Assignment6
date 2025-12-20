Assignment 6 Solution
---------------------

# Team Members

Benjamin Hikaru Pfister
Arthur Van Petegem

# GitHub link to your (forked) repository

...

# Task 1

1. Indicate WebIDs of the group members and the files corresponding to the profiles of the group members.

Ans: 
Arthur WebID: https://wiser-solid-xi.interactions.ics.unisg.ch/group8_pod2/profile/card#me
Benjamin WebID: https://wiser-solid-xi.interactions.ics.unisg.ch/Group8_pod/profile/card#me
Files: arthur-profile.ttl and benjamin-profile.ttl

2. Indicate the URL of group profile and the file that contains the group profile.

Ans: https://wiser-solid-xi.interactions.ics.unisg.ch/group8_pod2/profile/card#me
Files: group-info.ttl



# Task 2

1. Create a SPARQL query to retrieve the URI of the group to which you belong from your FOAF profile. Provide the query in the [`query_group.rq`](query_group.rq) file. 


2. Query the names of all the people in your distributed social graph (i.e., people you know directly or indirectly) using your profile as an entry point. To do this, you will need to write a navigational query (see lecture slides) and use link traversal (using the command comunica-sparql-link-traversal). Try running the query without link traversal as well and see what happens. Provide the query in the [`query_friends.rq`](query_friends.rq) file (see project README) and explain the results.

Ans: With link traversal comunica automatically follows the links from a profile to other profiles across the web. Without link traversal the query returns no results, with link traversal we found 7 people. This is because the query uses the (foaf:knows)+ property to find all relationships to find direct friends and friends of friends.


# Task 4

1. Which rules of Linked Data are applied to create the distributed knowledge graphs used in this assignment? Provide one concrete example for each rule you identify.

Ans: The assignment follows Tim Berners-Lee’s four Linked Data principles:

     URIs as names: Every entity is identified by a unique URI, such as our WebID (https://.../profile/card#me).

     HTTP access: These URIs are accessible via the HTTP protocol, allowing browsers and tools like Comunica to look them up.

     Standardized data: When looked up, the URIs return useful data in standard formats like RDF/Turtle.

     Links to others: The data includes links to other URIs, such as foaf:knows pointing to team members, which connects the isolated data into a distributed graph.

2. One of your colleagues states that a Solid pod in itself is represented as a knowledge graph. Do you agree with this statement? Explain briefly

Ans: Yes, I agree. A Solid Pod stores data using RDF triples (Subject-Predicate-Object), which inherently describe      
     relationships between entities. Since the data is structured as a network of connected nodes, linking internal resources (like a movie container) and external ones (like friends profiles), the Pod really does function as a personal knowledge graph.

3. One core idea behind Solid is to decouple applications from data. Explain in your own words what this means and what technical and societal implications you see.

Ans: Decoupling means that data resides in the user's personal Pod, while applications act just as interchangeable tools that 
     request access to read or modify that data. Technically, this allows different apps to operate on the same data without needing complex integrations, promoting interoperability. Societally, this restores data sovereignty: users own their digital identity and can switch service providers at any time without losing their history or data (preventing vendor lock-in).


