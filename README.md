CRUD API
This API allows you to insert, view, update, and delete

## API DESCRIPTION
This CRUD API is designed to facilitate Create, Read, Update, and Delete operations on a specific dataset or resource. 
It provides a set of endpoints that allow users to interact with MYSQL database named 'demo' with a table named 'names'.


## API ENDPOINT
The API consist of 4 endpoints:
   1. postName - This endpoint allows you to insert a new name into the database table named "names". The method used in postName is POST.
        * Required Parameters:
            > fname (string): First Name
            > lname (string): Last Name
   2. printName - This endpoint allows you to read and extract data from the database named "demo".  The method used in
                   printName is GET. 
        *Required Parameters:
            > there is no required parameters
   3. updateName - This endpoint enables use to update existing data in the database. The method used in updateName is POST.
        *Required Parameters:
            > 'id': Unique Identifier of each name or record on the database.
            > fname (string): First Name
            > lname (string): Last Name
   4. deleteName - This endpoint allows user to delete a name from database. The method used in deleteName is POST.
        *Required Parameters:
           > 'id': The unique Identifier of the name in the database that wll be deleted.
      

## REQUEST PAYLOADS
  1. postName  - {"lname":"enriquez", "fname":"joana"}
  2. printName  - This endpoint doesn't require request payload as it will automatically print or prompt the request payload.
  3. updateName -  {"id":7, "lname":"Enriquez-Cruz", "fname":"Jo-Ana" }
  4. deleteName - { "id":7 }


Explain the
structure of the request payload, including any required or optional fields.
You can use JSON examples to illustrate.


 


## Response


Describe the
structure of the API response, including possible status codes and JSON
examples.


 


## Usage


Provide code
examples or instructions on how to use your API.


 


## License


Mention the
license under which your API is distributed.


 


## Contributors


List
contributors or give credit to any external libraries or resources used.


 


## Contact
Information
