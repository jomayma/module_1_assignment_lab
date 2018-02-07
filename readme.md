Imagine you work at a Bitcoin exchange and you have customer information coming from another source: SSN, credit card and their bitcoin numbers. However, the file format is CSV and your exchange can only support JSON. Your task is to write a Node script to convert CSV into JSON.

A CSV file is like a table. It has the following structure in which the first line has the field names and the rest of the lines have the data:

id,first_name,last_name,email,gender,ip_address,ssn,credit_card,bitcoin,street_address
1,Ario,Noteyoung,anoteyoung0@nhs.uk,Male,99.5.160.227,509-86-9654,5602256742685208,179BsXQkUuC6NKYNsQkdmKQKbMBPmJtEHB,0227 Kropf Court
2,Minni,Endon,mendon1@netvibes.com,Female,213.62.229.103,765-11-9543,67613037902735554,135wbMcR98R6hqqWgEJXHZHcanQKGRPwE1,90 Sutteridge Way
...
The node script that will convert the customer-data.csv file into a JSON file. The 1st row of the CSV file acts as the keys/properties of the JSON object and the rest of the fields act as values. The JSON file must have an array with 1000 items. Output the JSON file in the same directory and name the file customer-data.json.

Here's an example of the JSON file structure which your Node program will need to produce:

[
  {
    "id": "1",
    "first_name": "Ario",
    "last_name": "Noteyoung",
    "email": "anoteyoung0@nhs.uk",
    "gender": "Male",
    "ip_address": "99.5.160.227",
    "ssn": "509-86-9654",
    "credit_card": "5602256742685208",
    "bitcoin": "179BsXQkUuC6NKYNsQkdmKQKbMBPmJtEHB",
    "street_address": "0227 Kropf Court"
  },
  {
    "id": "2",
    "first_name": "Minni",
    "last_name": "Endon",
    "email": "mendon1@netvibes.com",
    "gender": "Female",
    "ip_address": "213.62.229.103",
    "ssn": "765-11-9543",
    "credit_card": "67613037902735554",
    "bitcoin": "135wbMcR98R6hqqWgEJXHZHcanQKGRPwE1",
    "street_address": "90 Sutteridge Way"
  },
  ...