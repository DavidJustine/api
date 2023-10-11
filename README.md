"# api" 

# GitHub Activity


API for managing list of names in database. Consisting some endpoints for creating, reading, updating and deleting data records from database.


 


## API Description
This API allows the user to execute a basic CRUD(Create, Read, Update & Delete) operations in the database. Using this API, you can add, retrieve, update, and delete data name records from the database.


 


## API Endpoints
The API consists of these following endpoints

1. Inserting Name<br>
     ○ Endpoint /postName<br>
     ○ Method: POST<br>
     ○ Description: Insert a name in the database<br>
     ○ Request Payload:<br>
           {
            "lname":"hortizuela",
             "fname":"manny"
           }<br>
   
3.  Print  the name<br>
     ○ Endpoint /printName<br>
     ○ Method: POST<br>
     ○ Description: Print a name<br>
    
4. Get Name<br>
     ○ Endpoint /getName/{fname}/{lname}<br>
     ○ Method: GET<br>
     ○ Description: retrieve and display the name entered in the URL<br>

5. Update the Name<br>
     ○ Endpoint /updateName/{id}<br>
     ○ Method: PUT<br>
     ○ Description: Update a name in the database<br>
     ○ Request Payload:<br>
           {
             "lname":"wick",
              "fname":"john"
           }<br>

6. Delete the name<br>
     ○ Endpoint /deleteName<br>
     ○ Method: DELETE<br>
     ○ Description: Delete a name in the database<br>
     ○ Request Payload:<br>
           {
             "id":1
           }<br>

## Request Payload
```POST/postName```<br>
      • Endpoint for inserting name into the database<br>
      • Request payload structure (JSON)<br>
            {
             "lname":"hortizuela",
             "fname":"manny"
            } <br>
 ```PUT/updateName/{id}```<br>
       • Endpoint for updating name into the database<br>
       • Request payload structure (JSON)<br>
            {
             "id" : 1,
             "lname":"wick",
             "fname":"john"
            }<br>
```DELETE/deleteName```<br>
       • Endpoint for deleting name into the database<br>
       • Request payload structure (JSON)<br>
            {
             "id":1
            }<br>

## Response
The API responses follow a JSON format and includes these following structures:<br>
   • Success Response:<br>
      {
         "status": "success",
         "data": null
      }<br>

   • Error Response:<br>
      {
         "status": "error",
         "message": "Error message"
      }<br>
     
## Usage
Here are instructions how to use the endpoints of the API<br>
(Make sure that you have created a Database)<br>
(DB name: Demo, Table name: names, table contents: id, lname,fname)<br>

Open your Postman Software<br>
```postName```<br>
1. Set your method into POST<br>
2. Set your URL into 127.0.0.1/api/public/postName<br>
3. Insert the name in a JSON format in the request payload<br>
       {
         "lname":"hortizuela",
         "fname":"manny"
       } <br>
   ![image](https://github.com/DavidJustine/api/assets/147040193/94063373-4f6d-4b58-9929-c6dff21c4b46)<br>
   it should look like this<br>
4. click Send.<br>


```updateName```<br>
1. Set your method into PUT<br>
2. Set your URL into 127.0.0.1/api/public/updateName/{id}<br>
3. Insert the data in a JSON format in the request payload<br>
       {
         "id": "1",
         "lname":"hortizuela",
         "fname":"manny"
       }<br>
 ![Screenshot 2023-10-11 223401](https://github.com/DavidJustine/api/assets/147040193/4a5b1c6a-1417-4fbb-b559-6ba1947b9e54)<br>
 it should look like this<br>
4. Click send.<br>


```deleteName```<br>
1. Set your method into DELETE<br>
2. Set your URL into 127.0.0.1/api/public/deleteName<br>
3. Delete the data in a JSON format in the request payload<br>
       {
         "id": "1"
       }<br>
 ![Screenshot 2023-10-11 221259](https://github.com/DavidJustine/api/assets/147040193/76724050-6f6c-4715-98e5-c048f7b137b2)<br>
it should look like this<br>
4. Click send.<br>


## License
 ○ Apache License 2.0<br>
 ○ OrgStructure<br>


 


## Contributors
David Justine A. Javillonar - Initiated and created and pushed Git repository<br>
X'tynn J'ann S. Orpilla - Executed pulling the git repository from the github


 


## Contact Us
David Justine A. Javillonar | https://github.com/DavidJustine<br>
Email: davidjustine.javillonar@student.dmmmsu.edu.ph<br>

X'tynn J'ann S. Orpilla | https://github.com/TynOrpilla<br>
Email: xtynnjann.orpilla@student.dmmmsu.edu.ph
