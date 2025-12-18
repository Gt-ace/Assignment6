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

Ans:

2. One of your colleagues states that a Solid pod in itself is represented as a knowledge graph. Do you agree with this statement? Explain briefly

Ans:

3. One core idea behind Solid is to decouple applications from data. Explain in your own words what this means and what technical and societal implications you see.

Ans: 


