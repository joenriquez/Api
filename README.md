## CRUD API
This API allows you to insert, view, update, and delete

## API DESCRIPTION
This CRUD API is designed to facilitate Create, Read, Update, and Delete operations on a specific dataset or resource. 
It provides a set of endpoints that allow users to interact with MYSQL database named 'demo' with a table named 'names'.


## API ENDPOINT
The API consist of 4 endpoints:
   1. postName - This endpoint allows you to insert a new name into the database table named "names". The method used
                  in postName is POST.
        * Required Parameters:
            > fname (string): First Name
            > lname (string): Last Name
   3. printName - This endpoint allows you to read and extract data from the database named "demo".  The method used in
                   printName is GET. 
        *Required Parameters:
            > there is no required parameters
   4. updateName - This endpoint enables use to update existing data in the database. The method used in updateName is
                     POST.
        *Required Parameters:
            > 'id': Unique Identifier of each name or record on the database.
            > fname (string): First Name
            > lname (string): Last Name
   5. deleteName - This endpoint allows user to delete a name from database. The method used in deleteName is POST.
        *Required Parameters:
           > 'id': The unique Identifier of the name in the database that wll be deleted.
      

## REQUEST PAYLOADS
  1. postName  - {"lname":"enriquez", "fname":"joana"}
  2. printName  - This endpoint doesn't require request payload as it will automatically print or prompt the request
                  payload.
  3. updateName -  {"id":7, "lname":"Enriquez-Cruz", "fname":"Jo-Ana" }
  4. deleteName - { "id":7 }

## RESPONSE
   1. postName - { "status":"success","data":null }
   2. printName - { "status":"success","data": ["lname" : "hortizuela", "fname": "manny", "lname" : "enriquez",
                     "fname":"joana" ]
   3. updateName - { "status":"success","data":null }
   4. deleteName - { "status":"success","data":null }

## USAGE
   1. Open Xampp
   2. Create database named "demo"
   3. Create table named "names" and create columns 'id', 'fname', 'lname'
   4. Create a floder in the following directory: C://xampp/htdocs with the named 'api'.
   5. Install and open Postman
   6. Set HTTP method whether it is POST or GET.
   7. Enter the following URL for the endpoint:
       > postName -  localhost/api/public/postName
       > printName - localhost/api/public/printName
       > updateName - localhost/api/public/updateName
       > deleteName - localhost/api/public/deleteName
   8. In Postman there is a tab called 'Body tab', navigate to the body tab and input the json request payload. 

## LICENSE
There is no license used


## CONTRIBUTORS
Mr. Manny Hortizuela


## Contact
Email : enriquezjoana501@gmail.com
