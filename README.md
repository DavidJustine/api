"# api" 

# GitHub Activity


API for managing list of names in database. Consisting some endpoints for creating, reading, updating and deleting data records from database.


 


## API Description
This API allows the user to execute a basic CRUD(Create, Read, Update & Delete) operations in the database. Using this API, you can add, retrieve, update, and delete data name records from the database.


 


## API Endpoints
The API consists of these following endpoints

1. Inserting Name
     ○ Endpoint /postName
     ○ Method: POST
     ○ Description: Insert a name in the database
     ○ Request Payload:
           {
            "lname":"hortizuela",
             "fname":"manny"
           }
   
3.  Print  the name
     ○ Endpoint /printName
     ○ Method: POST
     ○ Description: Print a name
    
4. Get Name
     ○ Endpoint /getName/{fname}/{lname}
     ○ Method: GET
     ○ Description: retrieve and display the name entered in the URL

5. Update the Name
     ○ Endpoint /updateName/{id}
     ○ Method: PUT
     ○ Description: Update a name in the database
     ○ Request Payload:
           {
             "lname":"wick",
              "fname":"john"
           }

6. Delete the name
     ○ Endpoint /deleteName
     ○ Method: DELETE
     ○ Description: Delete a name in the database
     ○ Request Payload:
           {
             "id":1
           }

## Request Payload
```POST/postName```
      • Endpoint for inserting name into the database
      • Request payload structure (JSON)
            {
             "lname":"hortizuela",
             "fname":"manny"
            } 
 ```PUT/updateName/{id}```
       • Endpoint for updating name into the database
       • Request payload structure (JSON)
            {
             "id" : 1,
             "lname":"wick",
             "fname":"john"
            }
```DELETE/deleteName```
       • Endpoint for deleting name into the database
       • Request payload structure (JSON)
            {
             "id":1
            }

## Response
The API responses follow a JSON format and includes these following structures:
   • Success Response:
      {
         "status": "success",
         "data": null
      }

   • Error Response:
      {
         "status": "error",
         "message": "Error message"
      }
     
## Usage
Here are instructions how to use the endpoints of the API
(Make sure that you have created a Database)
(DB name: Demo, Table name: names, table contents: id, lname,fname)

Open your Postman Software 
```postName```
1. Set your method into POST
2. Set your URL into 127.0.0.1/api/public/postName
3. Insert the name in a JSON format in the request payload
       {
         "lname":"hortizuela",
         "fname":"manny"
       } 
   ![image](https://github.com/DavidJustine/api/assets/147040193/94063373-4f6d-4b58-9929-c6dff21c4b46)
   it should look like this
4. click Send.


```updateName```
1. Set your method into PUT
2. Set your URL into 127.0.0.1/api/public/updateName/{id}
3. Insert the data in a JSON format in the request payload
       {
         "id": "1",
         "lname":"hortizuela",
         "fname":"manny"
       }
 ![Screenshot 2023-10-11 223401](https://github.com/DavidJustine/api/assets/147040193/4a5b1c6a-1417-4fbb-b559-6ba1947b9e54)
 it should look like this
4. Click send.


```deleteName```
1. Set your method into DELETE
2. Set your URL into 127.0.0.1/api/public/deleteName
3. Delete the data in a JSON format in the request payload
       {
         "id": "1"
       }
 ![Screenshot 2023-10-11 221259](https://github.com/DavidJustine/api/assets/147040193/76724050-6f6c-4715-98e5-c048f7b137b2)
it should look like this
4. Click send.


## License
 ○ Apache License 2.0
 ○ OrgStructure


 


## Contributors
David Justine A. Javillonar - Initiated and created and pushed Git repository
X'tynn J'ann S. Orpilla - Executed pulling the git repository from the github


 


## Contact Us
David Justine A. Javillonar | https://github.com/DavidJustine
Email: davidjustine.javillonar@student.dmmmsu.edu.ph

X'tynn J'ann S. Orpilla | https://github.com/TynOrpilla
Email: xtynnjann.orpilla@student.dmmmsu.edu.ph
