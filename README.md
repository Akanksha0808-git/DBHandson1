# DBHandson1
Creating a database using Queries in  MongoShell

 <h3> 1-Create a database , give it name like ""Human_Resource"". Create a collection inside this named ""employee""</h3>
   
    Ans:- use Human_Resource
          db.employee.insertMany([]) 
          
<hr>

<h3>2-Query the collection ""employee"" and list all the documents</h3>
      
      Ans:-   db.employee.insertMany([]) 

<hr>
<h3>3-Query the collection ""employee"" and list the employees who are having salary more than 30000</h3>

    Ans:- db.employee.find({"salary":{$gt:"30000"}})

<hr>


<h3>4-Query the collection ""employee"" and list the employees who are having experience more than 2 years.
</h3>
      
     Ans:- db.employee.find({"salary"{$gt:"30000"}})

<hr>


<h3>5-Query the collection ""employee"" and list the employees who are graduated after 2015 and having experience more than 1 year </h3>


    Ans:-  db.employee.find({"yearGrad":{$gt:"2015"},"overallExp":{$gt:"1"}})

<hr>

<h3>6-The collection ""employee"" and update the salary of the employee whose salary is greater than 70000 to 65000.</h3>


     Ans:- db.employee.updateMany({"salary":{$gt:"70000"}},{$set:{"salary":"65000"}})

<hr>

<h3>7-Query Delete all the documents from ""employee"" where last company is Y"</h3>


     Ans:-db.employee.deleteMany({"lastCompany":"Y"})
 <hr>
