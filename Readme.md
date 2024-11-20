# **Zen Class Programme - Mongo DB Task**

1. The 7 Requirements namely Users, Codekata, Attendance, Topics, Taks, Company_Drives and Mentors are Created. Then the attachment has been added as a screenshot. 

2. Then 6 queries and their operation log to fetch those data. Screenshot of the Queries has been attached along with the code in the starting of the document for your reference.


## Database Creation

### 1. Users Creation

db.users.insertMany([

  { "userId": 1, "userName": "Sowmiya", "userEmail": "sowmiya@gmail.com", "mentorId": 1 },
  { "userId": 2, "userName": "Arun Kumar", "userEmail": "arun.kumar@gmail.com", "mentorId": 2 },
  { "userId": 3, "userName": "Priya Devi", "userEmail": "priya.devi@yahoo.com", "mentorId": 3 },
  { "userId": 4, "userName": "Vijay Raghavan", "userEmail": "vijay.raghavan@gmail.com", "mentorId": 4 },
  { "userId": 5, "userName": "Nithya Lakshmi", "userEmail": "nithya.lakshmi@hotmail.com", "mentorId": 5 },
  { "userId": 6, "userName": "Ravi Shankar", "userEmail": "ravi.shankar@outlook.com", "mentorId": 1 },
  { "userId": 7, "userName": "Anjali Ramesh", "userEmail": "anjali.ramesh@aol.com", "mentorId": 2 },
  { "userId": 8, "userName": "Karthik Srinivasan", "userEmail": "karthik.srinivasan@gmail.com", "mentorId": 3 },
  { "userId": 9, "userName": "Divya Nair", "userEmail": "divya.nair@yahoo.com", "mentorId": 4 },
  { "userId": 10, "userName": "Saravanan V", "userEmail": "saravanan.v@rediffmail.com", "mentorId": 5 },
  { "userId": 11, "userName": "Meera Krishnan", "userEmail": "meera.krishnan@gmail.com", "mentorId": 1 },
  { "userId": 12, "userName": "Suresh Babu", "userEmail": "suresh.babu@gmail.com", "mentorId": 2 },
  { "userId": 13, "userName": "Lakshmi Priya", "userEmail": "lakshmi.priya@aol.com", "mentorId": 3 },
  { "userId": 14, "userName": "Rajesh Sundaram", "userEmail": "rajesh.sundaram@yahoo.com", "mentorId": 4 },
  { "userId": 15, "userName": "Indira Nivedita", "userEmail": "indira.nivedita@outlook.com", "mentorId": 5 },
  { "userId": 16, "userName": "Vikram Shastri", "userEmail": "vikram.shastri@gmail.com", "mentorId": 1 },
  { "userId": 17, "userName": "Sanjana Reddy", "userEmail": "sanjana.reddy@rediffmail.com", "mentorId": 2 },
  { "userId": 18, "userName": "Pradeep Raj", "userEmail": "pradeep.raj@yahoo.com", "mentorId": 3 },
  { "userId": 19, "userName": "Kavitha Narayan", "userEmail": "kavitha.narayan@aol.com", "mentorId": 4 },
  { "userId": 20, "userName": "Siva Prakash", "userEmail": "siva.prakash@gmail.com", "mentorId": 5 },
  { "userId": 21, "userName": "Radhika Iyer", "userEmail": "radhika.iyer@gmail.com", "mentorId": 1 },
  { "userId": 22, "userName": "Anand Rajan", "userEmail": "anand.rajan@yahoo.com", "mentorId": 2 },
  { "userId": 23, "userName": "Chitra Subramanian", "userEmail": "chitra.subramanian@outlook.com", "mentorId": 3 },
  { "userId": 24, "userName": "Ganesh S", "userEmail": "ganesh.s@aol.com", "mentorId": 4 },
  { "userId": 25, "userName": "Geetha Devi", "userEmail": "geetha.devi@rediffmail.com", "mentorId": 5 },
  { "userId": 26, "userName": "Madhavan Suresh", "userEmail": "madhavan.suresh@gmail.com", "mentorId": 1 },
  { "userId": 27, "userName": "Jaya Lakshmi", "userEmail": "jaya.lakshmi@yahoo.com", "mentorId": 2 },
  { "userId": 28, "userName": "Vishal Ramakrishnan", "userEmail": "vishal.ramakrishnan@gmail.com", "mentorId": 3 },
  { "userId": 29, "userName": "Aishwarya Iyer", "userEmail": "aishwarya.iyer@aol.com", "mentorId": 4 },
  { "userId": 30, "userName": "Raj Kumar", "userEmail": "raj.kumar@hotmail.com", "mentorId": 5 }
])

``
db.getCollection('Users').find({});
```

### 2.codekata

``` db.getCollection("CodeKata").insertMany([
  { "_id": ObjectId("64fedb09c877bf3677214927"), "userId": 1, "problemSolved": 13 },
  { "_id": ObjectId("64fedb09c877bf3677214928"), "userId": 2, "problemSolved": 18 },
  { "_id": ObjectId("64fedb09c877bf3677214929"), "userId": 3, "problemSolved": 22 },
  { "_id": ObjectId("64fedb09c877bf3677214930"), "userId": 4, "problemSolved": 8 },
  { "_id": ObjectId("64fedb09c877bf3677214931"), "userId": 5, "problemSolved": 15 },
  { "_id": ObjectId("64fedb09c877bf3677214932"), "userId": 6, "problemSolved": 30 },
  { "_id": ObjectId("64fedb09c877bf3677214933"), "userId": 7, "problemSolved": 20 },
  { "_id": ObjectId("64fedb09c877bf3677214934"), "userId": 8, "problemSolved": 25 },
  { "_id": ObjectId("64fedb09c877bf3677214935"), "userId": 9, "problemSolved": 12 },
  { "_id": ObjectId("64fedb09c877bf3677214936"), "userId": 10, "problemSolved": 9 },
  { "_id": ObjectId("64fedb09c877bf3677214937"), "userId": 11, "problemSolved": 5 },
  { "_id": ObjectId("64fedb09c877bf3677214938"), "userId": 12, "problemSolved": 17 },
  { "_id": ObjectId("64fedb09c877bf3677214939"), "userId": 13, "problemSolved": 10 },
  { "_id": ObjectId("64fedb09c877bf3677214940"), "userId": 14, "problemSolved": 26 },
  { "_id": ObjectId("64fedb09c877bf3677214941"), "userId": 15, "problemSolved": 23 },
  { "_id": ObjectId("64fedb09c877bf3677214942"), "userId": 16, "problemSolved": 11 },
  { "_id": ObjectId("64fedb09c877bf3677214943"), "userId": 17, "problemSolved": 14 },
  { "_id": ObjectId("64fedb09c877bf3677214944"), "userId": 18, "problemSolved": 28 },
  { "_id": ObjectId("64fedb09c877bf3677214945"), "userId": 19, "problemSolved": 19 },
  { "_id": ObjectId("64fedb09c877bf3677214946"), "userId": 20, "problemSolved": 16 },
  { "_id": ObjectId("64fedb09c877bf3677214947"), "userId": 21, "problemSolved": 21 },
  { "_id": ObjectId("64fedb09c877bf3677214948"), "userId": 22, "problemSolved": 18 },
  { "_id": ObjectId("64fedb09c877bf3677214949"), "userId": 23, "problemSolved": 7 },
  { "_id": ObjectId("64fedb09c877bf3677214950"), "userId": 24, "problemSolved": 24 },
  { "_id": ObjectId("64fedb09c877bf3677214951"), "userId": 25, "problemSolved": 13 },
  { "_id": ObjectId("64fedb09c877bf3677214952"), "userId": 26, "problemSolved": 6 },
  { "_id": ObjectId("64fedb09c877bf3677214953"), "userId": 27, "problemSolved": 29 },
  { "_id": ObjectId("64fedb09c877bf3677214954"), "userId": 28, "problemSolved": 2 },
  { "_id": ObjectId("64fedb09c877bf3677214955"), "userId": 29, "problemSolved": 27 },
  { "_id": ObjectId("64fedb09c877bf3677214956"), "userId": 30, "problemSolved": 1 }
]); 
```

```
db.getCollection('CodeKata').find({});

```

### 3.Attendance


```
db.getCollection('UserTopics').insertMany([

  // Topic 1

  { "_id": ObjectId("64fedc53c877bf3677214944"), "userId": 1, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214945"), "userId": 2, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214946"), "userId": 3, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214947"), "userId": 4, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214948"), "userId": 5, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214949"), "userId": 6, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214950"), "userId": 7, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214951"), "userId": 8, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214952"), "userId": 9, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214953"), "userId": 10, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214954"), "userId": 11, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214955"), "userId": 12, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214956"), "userId": 13, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214957"), "userId": 14, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214958"), "userId": 15, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214959"), "userId": 16, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214960"), "userId": 17, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214961"), "userId": 18, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214962"), "userId": 19, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214963"), "userId": 20, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214964"), "userId": 21, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214965"), "userId": 22, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214966"), "userId": 23, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214967"), "userId": 24, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214968"), "userId": 25, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214969"), "userId": 26, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214970"), "userId": 27, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214971"), "userId": 28, "topicId": 1, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214972"), "userId": 29, "topicId": 1, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214973"), "userId": 30, "topicId": 1, "attended": false },

  // Topic 2

  { "_id": ObjectId("64fedc53c877bf3677214974"), "userId": 1, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214975"), "userId": 2, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214976"), "userId": 3, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214977"), "userId": 4, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214978"), "userId": 5, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214979"), "userId": 6, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214980"), "userId": 7, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214981"), "userId": 8, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214982"), "userId": 9, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214983"), "userId": 10, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214984"), "userId": 11, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214985"), "userId": 12, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214986"), "userId": 13, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214987"), "userId": 14, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214988"), "userId": 15, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214989"), "userId": 16, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214990"), "userId": 17, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214991"), "userId": 18, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214992"), "userId": 19, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214993"), "userId": 20, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214994"), "userId": 21, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214995"), "userId": 22, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214996"), "userId": 23, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214997"), "userId": 24, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677214998"), "userId": 25, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677214999"), "userId": 26, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215000"), "userId": 27, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215001"), "userId": 28, "topicId": 2, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215002"), "userId": 29, "topicId": 2, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215003"), "userId": 30, "topicId": 2, "attended": true },

  // Topic 3

  { "_id": ObjectId("64fedc53c877bf3677215004"), "userId": 1, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215005"), "userId": 2, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215006"), "userId": 3, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215007"), "userId": 4, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215008"), "userId": 5, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215009"), "userId": 6, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215010"), "userId": 7, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215011"), "userId": 8, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215012"), "userId": 9, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215013"), "userId": 10, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215014"), "userId": 11, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215015"), "userId": 12, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215016"), "userId": 13, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215017"), "userId": 14, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215018"), "userId": 15, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215019"), "userId": 16, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215020"), "userId": 17, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215021"), "userId": 18, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215022"), "userId": 19, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215023"), "userId": 20, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215024"), "userId": 21, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215025"), "userId": 22, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215026"), "userId": 23, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215027"), "userId": 24, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215028"), "userId": 25, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215029"), "userId": 26, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215030"), "userId": 27, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215031"), "userId": 28, "topicId": 3, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215032"), "userId": 29, "topicId": 3, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215033"), "userId": 30, "topicId": 3, "attended": false },

// Topic 4
  
  { "_id": ObjectId("64fedc53c877bf3677215034"), "userId": 1, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215035"), "userId": 2, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215036"), "userId": 3, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215037"), "userId": 4, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215038"), "userId": 5, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215039"), "userId": 6, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215040"), "userId": 7, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215041"), "userId": 8, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215042"), "userId": 9, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215043"), "userId": 10, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215044"), "userId": 11, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215045"), "userId": 12, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215046"), "userId": 13, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215047"), "userId": 14, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215048"), "userId": 15, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215049"), "userId": 16, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215050"), "userId": 17, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215051"), "userId": 18, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215052"), "userId": 19, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215053"), "userId": 20, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215054"), "userId": 21, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215055"), "userId": 22, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215056"), "userId": 23, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215057"), "userId": 24, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215058"), "userId": 25, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215059"), "userId": 26, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215060"), "userId": 27, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215061"), "userId": 28, "topicId": 4, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215062"), "userId": 29, "topicId": 4, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215063"), "userId": 30, "topicId": 4, "attended": false },

  // Topic 5

  { "_id": ObjectId("64fedc53c877bf3677215064"), "userId": 1, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215065"), "userId": 2, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215066"), "userId": 3, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215067"), "userId": 4, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215068"), "userId": 5, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215069"), "userId": 6, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215070"), "userId": 7, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215071"), "userId": 8, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215072"), "userId": 9, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215073"), "userId": 10, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215074"), "userId": 11, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215075"), "userId": 12, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215076"), "userId": 13, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215077"), "userId": 14, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215078"), "userId": 15, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215079"), "userId": 16, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215080"), "userId": 17, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215081"), "userId": 18, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215082"), "userId": 19, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215083"), "userId": 20, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215084"), "userId": 21, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215085"), "userId": 22, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215086"), "userId": 23, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215087"), "userId": 24, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215088"), "userId": 25, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215089"), "userId": 26, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215090"), "userId": 27, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215091"), "userId": 28, "topicId": 5, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215092"), "userId": 29, "topicId": 5, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215093"), "userId": 30, "topicId": 5, "attended": true },

  // Topic 6

  { "_id": ObjectId("64fedc53c877bf3677215094"), "userId": 1, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215095"), "userId": 2, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215096"), "userId": 3, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215097"), "userId": 4, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215098"), "userId": 5, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215099"), "userId": 6, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215100"), "userId": 7, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215101"), "userId": 8, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215102"), "userId": 9, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215103"), "userId": 10, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215104"), "userId": 11, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215105"), "userId": 12, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215106"), "userId": 13, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215107"), "userId": 14, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215108"), "userId": 15, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215109"), "userId": 16, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215110"), "userId": 17, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215111"), "userId": 18, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215112"), "userId": 19, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215113"), "userId": 20, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215114"), "userId": 21, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215115"), "userId": 22, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215116"), "userId": 23, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215117"), "userId": 24, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215118"), "userId": 25, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215119"), "userId": 26, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215120"), "userId": 27, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215121"), "userId": 28, "topicId": 6, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215122"), "userId": 29, "topicId": 6, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215123"), "userId": 30, "topicId": 6, "attended": false },

  // Topic 7

  { "_id": ObjectId("64fedc53c877bf3677215124"), "userId": 1, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215125"), "userId": 2, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215126"), "userId": 3, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215127"), "userId": 4, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215128"), "userId": 5, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215129"), "userId": 6, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215130"), "userId": 7, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215131"), "userId": 8, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215132"), "userId": 9, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215133"), "userId": 10, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215134"), "userId": 11, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215135"), "userId": 12, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215136"), "userId": 13, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215137"), "userId": 14, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215138"), "userId": 15, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215139"), "userId": 16, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215140"), "userId": 17, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215141"), "userId": 18, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215142"), "userId": 19, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215143"), "userId": 20, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215144"), "userId": 21, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215145"), "userId": 22, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215146"), "userId": 23, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215147"), "userId": 24, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215148"), "userId": 25, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215149"), "userId": 26, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215150"), "userId": 27, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215151"), "userId": 28, "topicId": 7, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215152"), "userId": 29, "topicId": 7, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215153"), "userId": 30, "topicId": 7, "attended": false },

  // Topic 8

  { "_id": ObjectId("64fedc53c877bf3677215154"), "userId": 1, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215155"), "userId": 2, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215156"), "userId": 3, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215157"), "userId": 4, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215158"), "userId": 5, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215159"), "userId": 6, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215160"), "userId": 7, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215161"), "userId": 8, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215162"), "userId": 9, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215163"), "userId": 10, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215164"), "userId": 11, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215165"), "userId": 12, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215166"), "userId": 13, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215167"), "userId": 14, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215168"), "userId": 15, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215169"), "userId": 16, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215170"), "userId": 17, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215171"), "userId": 18, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215172"), "userId": 19, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215173"), "userId": 20, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215174"), "userId": 21, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215175"), "userId": 22, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215176"), "userId": 23, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215177"), "userId": 24, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215178"), "userId": 25, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215179"), "userId": 26, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215180"), "userId": 27, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215181"), "userId": 28, "topicId": 8, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215182"), "userId": 29, "topicId": 8, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215183"), "userId": 30, "topicId": 8, "attended": true },

  // Topic 9

  { "_id": ObjectId("64fedc53c877bf3677215184"), "userId": 1, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215185"), "userId": 2, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215186"), "userId": 3, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215187"), "userId": 4, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215188"), "userId": 5, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215189"), "userId": 6, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215190"), "userId": 7, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215191"), "userId": 8, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215192"), "userId": 9, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215193"), "userId": 10, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215194"), "userId": 11, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215195"), "userId": 12, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215196"), "userId": 13, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215197"), "userId": 14, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215198"), "userId": 15, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215199"), "userId": 16, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215200"), "userId": 17, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215201"), "userId": 18, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215202"), "userId": 19, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215203"), "userId": 20, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215204"), "userId": 21, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215205"), "userId": 22, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215206"), "userId": 23, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215207"), "userId": 24, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215208"), "userId": 25, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215209"), "userId": 26, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215210"), "userId": 27, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215211"), "userId": 28, "topicId": 9, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215212"), "userId": 29, "topicId": 9, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215213"), "userId": 30, "topicId": 9, "attended": false },

  // Topic 10

  { "_id": ObjectId("64fedc53c877bf3677215214"), "userId": 1, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215215"), "userId": 2, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215216"), "userId": 3, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215217"), "userId": 4, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215218"), "userId": 5, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215219"), "userId": 6, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215220"), "userId": 7, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215221"), "userId": 8, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215222"), "userId": 9, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215223"), "userId": 10, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215224"), "userId": 11, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215225"), "userId": 12, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215226"), "userId": 13, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215227"), "userId": 14, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215228"), "userId": 15, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215229"), "userId": 16, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215230"), "userId": 17, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215231"), "userId": 18, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215232"), "userId": 19, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215233"), "userId": 20, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215234"), "userId": 21, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215235"), "userId": 22, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215236"), "userId": 23, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215237"), "userId": 24, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215238"), "userId": 25, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215239"), "userId": 26, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215240"), "userId": 27, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215241"), "userId": 28, "topicId": 10, "attended": true },
  { "_id": ObjectId("64fedc53c877bf3677215242"), "userId": 29, "topicId": 10, "attended": false },
  { "_id": ObjectId("64fedc53c877bf3677215243"), "userId": 30, "topicId": 10, "attended": true }
]);

```
db.getCollection('Attendance').find({});

### 4. Topics

```
db.getCollection('Topics').insertMany([
  {
    "_id": { "$oid": "64fee15bc877bf3677214a9d" },
    "topicId": 1,
    "topic": "MERN Stack Overview",
    "topicDate": "2021-02-15"
  },
  {
    "_id": { "$oid": "64fee15bc877bf3677214a9e" },
    "topicId": 2,
    "topic": "Building REST APIs with Node.js and Express",
    "topicDate": "2021-03-01"
  },
  {
    "_id": { "$oid": "64fee15bc877bf3677214a9f" },
    "topicId": 3,
    "topic": "React vs Angular: Key Differences",
    "topicDate": "2021-04-10"
  },
  {
    "_id": { "$oid": "64fee15bc877bf3677214aa0" },
    "topicId": 4,
    "topic": "State Management in React using Redux",
    "topicDate": "2021-05-20"
  },
  {
    "_id": { "$oid": "64fee15bc877bf3677214aa1" },
    "topicId": 5,
    "topic": "MongoDB Data Modeling and Optimization",
    "topicDate": "2021-06-12"
  },
  {
    "_id": { "$oid": "64fee15bc877bf3677214aa2" },
    "topicId": 6,
    "topic": "Angular Services and Dependency Injection",
    "topicDate": "2021-07-14"
  },
  {
    "_id": { "$oid": "64fee15bc877bf3677214aa3" },
    "topicId": 7,
    "topic": "Authentication and Authorization in MERN",
    "topicDate": "2021-08-05"
  },
  {
    "_id": { "$oid": "64fee15bc877bf3677214aa4" },
    "topicId": 8,
    "topic": "Integrating MongoDB with Express and Node.js",
    "topicDate": "2021-09-18"
  },
  {
    "_id": { "$oid": "64fee15bc877bf3677214aa5" },
    "topicId": 9,
    "topic": "Optimizing Performance in MERN Applications",
    "topicDate": "2021-10-21"
  },
  {
    "_id": { "$oid": "64fee15bc877bf3677214aa6" },
    "topicId": 10,
    "topic": "Testing MERN and MEAN Applications",
    "topicDate": "2021-11-12"
  }
]);
```
db.getCollection('Topics').find({});

```


### 5. Tasks

```
db.getCollection('Tasks').insertMany(
[
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 1,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 2,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": false
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 3,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 4,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 5,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 6,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 7,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 8,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 9,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 10,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 11,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": false
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 12,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 13,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 14,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": false
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 15,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 16,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 17,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": false
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 18,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 19,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 20,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 21,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 22,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 23,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 24,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 25,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": false
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 26,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 27,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 28,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 29,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 1,
    "topicId": 1,
    "userId": 30,
    "task": "MERN Stack.",
    "dueDate": "2021-02-20",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 1,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 2,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": false
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 3,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": false
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 4,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 5,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 6,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 7,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 8,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 9,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 10,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 11,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 12,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": false
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 13,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 14,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 15,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 16,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 17,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 18,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 19,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 20,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 21,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 22,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 23,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 24,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 25,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": false
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 26,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 27,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 28,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 29,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": true
  },
  {
    "taskId": 2,
    "topicId": 2,
    "userId": 30,
    "task": "Build a REST API using Node.js and Express.",
    "dueDate": "2021-03-05",
    "submitted": false
  }

  {
    "taskId": 3,
    "topicId": 3,
    "userId": 1,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 2,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 3,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 4,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 5,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 6,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 7,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 8,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 9,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 10,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 11,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 12,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 13,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 14,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 15,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 16,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 17,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 18,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 19,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 20,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 21,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 22,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": false
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 23,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 24,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 25,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 26,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 27,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 28,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 29,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
  {
    "taskId": 3,
    "topicId": 3,
    "userId": 30,
    "task": "React vs Angular: Key Differences",
    "dueDate": "2021-04-15",
    "submitted": true
  },
{
    "taskId": 4,
    "topicId": 4,
    "userId": 1,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 2,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 3,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 4,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 5,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 6,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 7,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 8,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 9,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 10,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": false
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 11,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": false
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 12,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 13,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 14,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 15,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 16,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 17,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 18,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 19,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 20,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 21,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 22,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": false
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 23,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": false
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 24,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 25,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 26,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 27,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 28,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 29,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
  {
    "taskId": 4,
    "topicId": 4,
    "userId": 30,
    "task": "State Management in React using Redux",
    "dueDate": "2021-05-30",
    "submitted": true
  },
{
    "taskId": 5,
    "topicId": 5,
    "userId": 1,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": false
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 2,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 3,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 4,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 5,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 6,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 7,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 8,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 9,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 10,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 11,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 12,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 13,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 14,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 15,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 16,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 17,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 18,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 19,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 20,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 21,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 22,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 23,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 24,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 25,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 26,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": false
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 27,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": false
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 28,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 29,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": false
  },
  {
    "taskId": 5,
    "topicId": 5,
    "userId": 30,
    "task": "MongoDB Data Modeling and Optimization",
    "dueDate": "2021-06-20",
    "submitted": true
  }
]);
```

db.getCollection('Tasks').find({});

### 6. company-drives

db.getCollection('Company-Drives').insertMany([
  {
    "userId": 13,
    "driveDate": "2020-10-04T00:00:00.000Z",
    "company": "Google"
  },
  {
    "userId": 25,
    "driveDate": "2021-01-15T00:00:00.000Z",
    "company": "Facebook"
  },
  {
    "userId": 7,
    "driveDate": "2021-02-25T00:00:00.000Z",
    "company": "Amazon"
  },
  {
    "userId": 18,
    "driveDate": "2021-03-10T00:00:00.000Z",
    "company": "Microsoft"
  },
  {
    "userId": 9,
    "driveDate": "2021-04-21T00:00:00.000Z",
    "company": "Apple"
  },
  {
    "userId": 22,
    "driveDate": "2021-05-05T00:00:00.000Z",
    "company": "Netflix"
  },
  {
    "userId": 4,
    "driveDate": "2021-06-18T00:00:00.000Z",
    "company": "Spotify"
  },
  {
    "userId": 11,
    "driveDate": "2021-07-02T00:00:00.000Z",
    "company": "Twitter"
  },
  {
    "userId": 30,
    "driveDate": "2021-08-14T00:00:00.000Z",
    "company": "Slack"
  },
  {
    "userId": 15,
    "driveDate": "2021-09-25T00:00:00.000Z",
    "company": "Adobe"
  }
]);

```
db.getCollection('Company_Drives').find({});
```

### 7. Mentors

```
db.getCollection('Mentors').insertMany([
  {
    "mentorId": 1,
    "mentorName": "Manikandan Anbazhagan",
    "mentorEmail": "manikandan@gmail.com"
  },
  {
    "mentorId": 2,
    "mentorName": "Ameer Hamza",
    "mentorEmail": "ameer.hamza@gmail.com"
  },
  {
    "mentorId": 3,
    "mentorName": "Revathi Mary",
    "mentorEmail": "revathi.mary@gmail.com"
  },
  {
    "mentorId": 4,
    "mentorName": "Zakir Hussein",
    "mentorEmail": "zakir.hussein@gmail.com"
  },
  {
    "mentorId": 5,
    "mentorName": "Sofia Fatima",
    "mentorEmail": "sofia.fatima@gmail.com"
  },
  {
    "mentorId": 6,
    "mentorName": "Benedict Raj",
    "mentorEmail": "benedict.raj@gmail.com"
  },
  {
    "mentorId": 7,
    "mentorName": "Sarah Mary",
    "mentorEmail": "sarah.mary@gmail.com"
  }
]);

```
db.getCollection('Mentors').find({});
```




# Queries 


### 1. Find all the topics and tasks which are thought in the month of October


```
db.topics.find({
  "topicDate": {
    "$gte": ISODate("2021-02-15T00:00:00.000Z"),
    "$lt": ISODate("2021-08-01T00:00:00.000Z")   
});


```
db.tasks.find({
  "dueDate": {
    "$gte": ISODate("2021-02-20T00:00:00.000Z"),
    "$lt": ISODate("2021-07-02T00:00:00.000Z")
  }
});



### 2. Find all the company drives which appeared between 15 oct-2020 and 31-oct-2020

db.company_drives.find({
  "driveDate": {
    "$gte": ISODate("2020-10-04T00:00:00.000Z"), 
    "$lt": ISODate("2021-09-25T00:00:00.000Z")   
  }
});

```
{
    "userId": 13,
    "driveDate": "2020-10-04T00:00:00.000Z",
    "company": "Google"
  },
  {
    "userId": 25,
    "driveDate": "2021-01-15T00:00:00.000Z",
    "company": "Facebook"
  },
  {
    "userId": 7,
    "driveDate": "2021-02-25T00:00:00.000Z",
    "company": "Amazon"
  },
  {
    "userId": 18,
    "driveDate": "2021-03-10T00:00:00.000Z",
    "company": "Microsoft"
  },
  {
    "userId": 9,
    "driveDate": "2021-04-21T00:00:00.000Z",
    "company": "Apple"
  },
  {
    "userId": 22,
    "driveDate": "2021-05-05T00:00:00.000Z",
    "company": "Netflix"
  },
  {
    "userId": 4,
    "driveDate": "2021-06-18T00:00:00.000Z",
    "company": "Spotify"
  },
  {
    "userId": 11,
    "driveDate": "2021-07-02T00:00:00.000Z",
    "company": "Twitter"
  },
  {
    "userId": 30,
    "driveDate": "2021-08-14T00:00:00.000Z",
    "company": "Slack"
  },
  {
    "userId": 15,
    "driveDate": "2021-09-25T00:00:00.000Z",
    "company": "Adobe"
  }

```

### 3. Find all the company drives and students who are appeared for the placement.
```
db["Company-Drives"].aggregate([
  {
    $lookup: {
      from: "users",                 
      localField: "students_appeared",
      foreignField: "_id",              
      as: "students"                 
    }
  }
])

```
{
  _id: ObjectId('67388eaa7fef43c5884f0e47'),
  userId: 13,
  driveDate: '2020-10-04T00:00:00.000Z',
  company: 'Google',
  students: [
  "userId": 13,
  "userName": "Lakshmi Priya",
  "userEmail": "lakshmi.priya@aol.com",
  "mentorId": 3
]
}
{
  _id: ObjectId('67384f8b7fef43c5884f0da0'),
  userId: 25,
  driveDate: '2021-01-15T00:00:00.000Z',
  company: 'Facebook',
  students: [
  "userId": 24,
  "userName": "Ganesh S",
  "userEmail": "ganesh.s@aol.com",
  "mentorId": 4
]
}
{
  _id: ObjectId('67384f8b7fef43c5884f0d8f'),
  userId: 7,
  driveDate: '2021-02-25T00:00:00.000Z',
  company: 'Amazon',
  students: [
  "userId": 7,
  "userName": "Anjali Ramesh",
  "userEmail": "anjali.ramesh@aol.com",
  "mentorId": 2
]
}

### 4.Find the number of problems solved by the user in codekata
```
db.CodeKata.find({}, { userId: 1, problemSolved: 1, _id: 0 })

{
  userId: 1,
  problemSolved: 13
}

{
  userId: 2,
  problemSolved: 18
}

{
  userId: 3,
  problemSolved: 22
}
```


### 5.Find all the mentors with who has the mentee's count more than 15
```
db.Mentors.find({
  $expr: {
    $gt: [
      { $size: { $ifNull: ["$mentees", []] } },  
      12  
    ]
  }
})

{
  _id: ObjectId('673890b27fef43c5884f0e55'),
  mentorId: 5,
  mentorName: 'Sofia Fatima',
  mentorEmail: 'sofia.fatima@gmail.com',
  mentees: [
    1,
    2,
    3,
    4,
    5,
    6,
    7,
    8,
    9,
    10,
    11,
    12,
    13
  ]
}
```

### 6. Find the number of users who are absent and task is not submitted  between 15 oct-2020 and 31-oct-2020

```
db.getCollection('Attendence').aggregate(
  [
    {
      $lookup: {
        from: 'Topics',
        localField: 'topicId',
        foreignField: 'topicId',
        as: 'Absent'
      }
    },
    {
      $lookup: {
        from: 'Tasks',
        localField: 'userId',
        foreignField: 'userId',
        as: 'Task-notSubmitted'
      }
    },
    {
      $unwind: { path: '$Task-notSubmitted', preserveNullAndEmptyArrays: true }
    },
    {
      $unwind: { path: '$Absent', preserveNullAndEmptyArrays: true }
    },
    {
      $match: {
        attended: false,
        'Absent.topicDate': {
          $gte: new Date('2021-02-15'),
          $lte: new Date('2021-10-15')
        },
        'Task-notSubmitted.dueDate': {
          $gte: new Date('2021-02-15'),
          $lte: new Date('2021-10-15')
        },
        'Task-notSubmitted.submitted': false
      }
    },
    {
      $group: {
        _id: '$userId' 
      }
    },
    {
      $count: 'absentAndTaskNotSubmitted' 
  ],
  { maxTimeMS: 60000, allowDiskUse: true }
);

