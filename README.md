"# api"

# API Name

JSON  with Database Integration
 
-Brief Description
- This API endpoint facilitates clients in sending organized data to a server for the purpose of creating or modifying records. The data is transmitted in JSON format, providing flexibility and convenience in handling. Following processing, the server responds with an HTTP status code and the required JSON. It finds application in tasks such as user registration, data modifications, and customized workflows, all under a secure authentication system. Please consult the official documentation for details on endpoint prerequisites and protocols for handling errors.
 

## API
- Description
- API stands for Application Programming Interface. It's a set of rules and protocols that allows different software applications to communicate and interact with each other. APIs enable the exchange of data an functionality between different programs or systems, enabling them to work together seamlessly. They are essential for enabling the integration of different services and applications, making it possible for them to share information and perform tasks in a coordinated way. APIs are used in a wide range of applications, from web development to mobile apps and even in hardware communication.


## API
Endpoints

Endpoint: /postName
http://127.0.0.1/api/public/postName

- Method: 
- Function: Inserts a new name into the database.
- Required Parameters (in JSON body):
   - fname: The first name.
   - lname: The last name.

Endpoint: /printName
http://127.0.0.1/api/public/printName

- Method: 
- Function: Always returns a predefined set of names in JSON format.
- No Required Parameters.

Endpoint: /updateName
http://127.0.0.1/api/public/updateName

- Method: PUT
- Function: Updates an existing name in the database.
- Required Parameters (in JSON body):
   - id: The ID of the record to be updated.
   - fname: The updated first name.
   - lname: The updated last name.

Endpoint: /deleteName
http://127.0.0.1/api/public/deleteName

- Method: DELETE
- Function: Deletes a name from the database based on the provided ID.
- Required Parameters (in JSON body):
   - id: The ID of the record to be deleted.

## Request
Payload

JSON Payload Name:
- JSON Payload postName:
- Request payload:
- {
  "lname":"hortizuela",
   "fname":"manny"
}

JSON Payload printName:
 
Request payload:

JSON Payload updateName:

- Request payload:
- {
  "id":1,
  "lname":"wick",
   "fname":"john"
}

JSON Payload deleteName:

- Request payload:
- {
  "id":1
}


## Response
JSON Payload Name:

- Response payload:
- {
         "status":"success","data":null
}

JSON Payload printName:

- Response payload:
- {
         "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"]
}


JSON Payload updateName:

- Response payload:
- {
         "status":"success","data":null
}


JSON Payload deleteName:

- Response payload:
- {
         "status":"success","data":null
}


## Usage
Follow these steps to manipulate database information using man and the API endpoints:

1. Launch postman:
Ensure that man is installed and operational on your system.

2. Send a  Request to Insert Data:
To insert data into the database via the /api/public/postName endpoint:

Choose the HTTP method as .
Input the URL: http://127.0.0.1/api/public/postName.
Within the request body, specify the parameters fname and lname along with the desired values for insertion.
Click "Send" to dispatch the request.

3.Send a  Request to Update Data:
To update existing database entries using the /api/public/updateName endpoint:

Select the HTTP method as .
Enter the URL: http://127.0.0.1/api/public/updateName.
In the request body, include the parameters id, fname, and lname, along with the updated values.
Click "Send" to submit the request.

4.Send a  Request to Print Data:
To showcase database data using the /api/public/printName endpoint:

Opt for the HTTP method as .
Specify the URL: http://127.0.0.1/api/public/printName.
Keep the request body empty as no additional parameters are required.
Click "Send" to transmit the request.

5. Send a  Request to Delete Data:
To remove data from the database through the /api/public/deleteName endpoint:

Set the HTTP method to .
Enter the URL: http://127.0.0.1/api/public/deleteName.
In the request body, include the parameter id with the ID of the data you intend to delete.

Click "Send" to initiate the request.


## License

No License 


## Contributors

Sir Manny Hortizuela
provided:

- some codes
- database structure
- payloads
- etc.


## Contact
Include contact
information for inquiries or support.

Heavrian Jim N. Ruiz
- heavrianjim.ruiz@student.dmmmsu.edu.ph
- 09310405247
