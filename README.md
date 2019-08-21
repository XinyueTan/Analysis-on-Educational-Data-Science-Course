# Project Discription

## Background

The data sets in this project come from a seven week educational data science course. I have access to data from two iterations of this course, one in 2014 and one in 2015. The course content is disaggregated, e.g.: Students choose the order in which they wish to tackle each unit. Students complete one unit each week for six weeks, in the seventh week all students must sit the same final exam. 

#### scores.csv 

This data set contains the unit choices, time spent on each unit in minutes and scores for each unit students recieved. It also contains final exam scores. All scores are represented at a proportion of the overall possible score (0 - 1).

#### tweets.csv

Permission was recieved from the students in this course to collect their tweets during the course. This data set contains those tweets, the week in which they were tweeted and if the tweet was a reply to another student in the class.**
** These are real Tweets from the wild, collected by the [Sentiment140](http://help.sentiment140.com/home) team at Stanford. I have attempted to clean them of anything offensive but may have missed something so be aware if you plan on reading the text.



## Goal of the analysis

In this project, I will be working towards building several **social network diagrams** (graphs/sociograms) of the 2014 class and 2015 class for the instructors and then analyzing both centrality measures and clusters within the network. I will identify isolated students in both classes, given that there is an observed correlation between an individuals' connectivity to peers and their overall academic success. With the meaningful interpretation of the structure of the network, teachers can give interventions to prevent students' dropout and increase the overall connectivity in class.

### Social Network for class 2014 VS class 2015

Class 2014             |  Class 2015
:-------------------------:|:-------------------------:
![](https://user-images.githubusercontent.com/46146748/63467190-dd329780-c432-11e9-9574-452f77962049.png)  |  ![](https://user-images.githubusercontent.com/46146748/63467242-fb989300-c432-11e9-9e22-b32446ab94cb.png)

### Visualizations of Cliques using Springlass Package
Springlass for Class 2014             |  Springlass for Class 2015
:-------------------------:|:-------------------------:
![](https://user-images.githubusercontent.com/46146748/63468616-5b446d80-c436-11e9-87c2-5f3cf36b429a.png)  |  ![](https://user-images.githubusercontent.com/46146748/63468705-816a0d80-c436-11e9-9ae7-bad52305e6e7.png)


In the second part, I will be generating several **predictions of students' performance for the instructor**. ANOVA test will be used to determine unit differences in terms of time spent on each unit and scores earned on each unit. Then, the class 2014 and class 2015 are compared. The linear regression is modeled to use scores for each unit to predict final exam scores. The ability to predict what a student is likely to get in the final exam in the future so that interventions can be tailored to them (e.g.: provide extra tutorial for students who are likely to fail the course) is an investment.

### Visualizations of relationships
Boxplot for Unit and Minute             |  Boxplot for Unit and Score  
:-------------------------:|:-------------------------:
![](https://user-images.githubusercontent.com/46146748/63469634-b37c6f00-c438-11e9-9fce-2bc08b83dc36.png)  |  ![](https://user-images.githubusercontent.com/46146748/63469676-ca22c600-c438-11e9-827c-de27b286f122.png)


## Related Materials
### Information about Social Network Analysis

Social network analysis (SNA) can be used to address research questions related to the level of participant engagement, identification of central participants and isolated students. Also, SNA provides instructors with the capacity to visualize group cohesion, network density, and evaluate the impact of intervention strategies on student engagement and connectivity by evaluating the evolution of participant relationships within discussions forums, 

#### Definitions and concepts
  * Isolated students: appear as nodes with no connections in terms of social and academic. Connections between nodes are weighted according to the number of posts and replies made between the participants
     * In the world of online learning, a participant who has submitted a post but no other participants have responded can be indicated as an isolated user.
     * In the world of online learning, attrition rates are frequently reported as higher than their on-campus counterparts. This has in part, been attributed to a lack of connectivity that is both social and academic, with fellow learners and the institution. Thus, any aids that can be afforded to forum facilitators to more accurately identify students that have not connected or have disengaged with the learning network early in their academic study, may assist with addressing concerns related to online attrition. 

  * Sub-groups or cliques: may indicate strong bonding among a core set of students. However, the formation of these strong cliques can be to the detriment of other actors attempting to engage. The formation of these groups can also limit the diversity of engagement with peers. 
     * In large class forums students will form cliques based on perceived academic potential. An effective strategy may include 1) assigning participants to new groups and establishing additional group specific discussion forums. 
      * Encourage participants to interact across multiple cliques (i.e. bridge structural holes) to foster intergroup idea sharing.
      
### Related Readings
[Bakharia, A., & Dawson, S. (2011). SNAPP: A Bird’S-eye View of Temporal Participant Interaction. In Proceedings of the 1st International Conference on Learning Analytics and Knowledge (pp. 168–173). Banff, Alberta, Canada:ACM.](https://doi.org/10.1145/2090116.2090144)

[Hanneman, R. & Riddle, M. (2005). Introduction to Social Network Methods. Riverside, CA:  University of California, Riverside](http://faculty.ucr.edu/~hanneman/)  
  * [Chapter 10: Centrality & Power](http://faculty.ucr.edu/~hanneman/nettext/C10_Centrality.html)  
  * [Chapter 11: Cliques & Subgroups](http://faculty.ucr.edu/~hanneman/nettext/C11_Cliques.html) 



## Author
[Katherine Tan](www.linkedin.com/in/katherine-tan-2019), M.S student in Learning Analytics at Teachers College, Columbia University
