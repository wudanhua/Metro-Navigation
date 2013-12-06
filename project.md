MetroNavigation

Introduction

MetroNavigation is planned to be an application based on already existing Kana, a mobile application designed for identifying location at Metropolia UAS Alberga campus. The core system enables a user to see their location but after being enhanced there will be several more features such are:

a. Navigation. We consider it to be one of the major benefits of the system. Nor only it makes life of users easier, but also it can be used by visitors, who do not have an account in the system.

b. Search for other users location. This feature is especially helpful for students, who have an appointment with a teacher.  One can find another user, and see their status available/busy/away.

c. Number of people at a particular place. Basically, it means that a user can check how many of other users are available/busy  in a classroom/library/cafeteria. 

d. Mark friends as favourites. Users can keep in touch with each other by viewing on the map where their friends are.

Our enhanced application is plain and handy, easy to use by anyone who has a smartphone, except for iOs users due to the Apple policies. Nevertheless, for anyone using mobile gadgets based on Android, we guarantee the application to be efficient, fast, and reliable.



2.User Groups Definition


1.	Visitor is a user that has not registered yet. They can open the application, but they cannot log in. They can also navigate.
2.	User is one who has an account. They are entitled to check in, see location of other users, find other users, and see number of people in places, navigate to a classroom.

Use Cases and Primary Actors

| Primary Actor	| Use Cases |
| ---- | ---- |
Visitor	 | 1.	Navigate to a classroom. |
 | 2.	Choose a classroom. |
User	| 1.	Log in |
 | 2.	Log out |
 | 3.	Check in |
 | 4.	See location of other users |
 | 5.	Find other users |
 | 6.	See a number of people available |
 | 7.	Navigate to a class room |
 | 8.	Mark friends as favorites |
 | 9.	Choose a classroom |
 | 10.	Put a status available/busy/away |




User scenario.
1. Initial state:
 |1. The client has established the Internet connection.
        2. The client has started a browser.
        3. The client has opened the web page.
2. Normal flow:
        1. The client logs in.
        2. The client browses sandwiches.
        3. The client selects a sandwich with cheese.
3. Exceptions:
        1. No connection.
        2. Login fails.
        3. No sandwiches with cheese left.
4. Other activities at the same time:
        1. The client sees recommendations.
5. The end:
        1. The client checks out.

##use case diagram

![fallback text](UseCaseDiagram.png)






System architecture

1. Log in. A Username and a password are needed, aunthentification response.

2. Location. Get user's location and other users' location - provided by Kana.
3. Navigation is a module, which provides a user with the shortest route to some place, a map, a route on the map.

4. Database where all information about users' accounts, room's number stored.



Requirements
Functional system requirements

1. Log in. A username and a password required, they are stored in the Database, and later on checked whether they are valid.
2. Check in. A user shares their location with others. Kana is used.
3. Set the status. A user chooses his status to be available/busy/away. Location is required, Kana is used.
4. Search for a classroom. Database and Kana are used.
5. Navigate to a classroom. Database, location, navigation are used.
6. See location of other users. Database, location are used.
7. Find other users. Database is used.
8. Mark friends as favorites.Database is used.
9. See a number of people available. Kana and Database are used.
10. Log out. Database is used.

Non-functional system requirements

1. Usability
To ensure that the system is easy to use our application is based on already exisiting application Kana, which proved to be handy. We have concluded, that the more simple the appplication is the better it is. Nevertheless, it is powerful enough to provide  our users with an execellent service, and store all information needed. 

On the front page there are two options, either to log in, or to proceed without it as a visitor. So nor only registered users can benefit from the application. 

2.Reliability

All user's information will be protected and completely private. No one except for the user can access it. 

The possible system failures are:
    1. Invalid ID or password-->Log in again, renew a password, register.
    2. Connection fail--> restart the application, check Internet connection.

3.Efficiency    
Although there are many users, especially on school time, we can ensure that average time that takes one to update is 5 seconds. This estimation is based on the fact that Metropolia Campus is equipped with fast Internet connection everywhere.


User interface

When user just open the application, log in is required. If the log in unsuccessful, it will give the "try again" option. After log in successfully, user can choose " Friends", "Teacher", "Classroom", "Library", "cafeteria".

"Friends" button is going to show the user's friends list, and user can add, delete, add as favourite. In the friends list, it is going to show the "favourite" friends first. In this view, database is used. After choosing a friend, the location of the friend will be showed in the school's map. Meanwhile, user can select "Route there" to get the shortest route to the friend on the map. Database, Kana, navigation are used.

When user click "Teacher" button, it will show teachers that are teaching cunrrentlly loged in user and a "Search" box. Database is used. After user choose one of the teachers, program will give the teacher's status(busy, available,away), office number. Location and database needed. User can navigate to the teacher from curent location. Navigation and location are used.

"Classroom" button is going to show the user's next classroom on the map and the shortest route to there. In this view, application is using database, Kana, and navigation. 

"Library", "Cafeteria" buttons are having the same function. Database, location, and navigation are required. When user click one of those buttons, applicaiton will show a number of users in that area. So user can decide whether to go there or not, depending on how many people there are. Also user can use our application to navigate to the Cafeteria or Library. At this point,  database, Kana, and navigation are used.



    
##flowchart
![fallback text](Flowchart.png)
