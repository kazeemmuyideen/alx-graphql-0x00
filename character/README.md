GraphQuest: Exploring and Implementing GraphQL
📌 Project Overview
This project focuses on writing GraphQL queries to fetch data for specific characters from a given API endpoint. The task involves retrieving detailed information about characters using their unique IDs.

We specifically query for characters with the following IDs: 1, 2, 3, and 4, and extract details such as:

id

name

status

species

type

gender

📂 Project Structure
|pgsql                              |
|Copy                               |
|Edit                               |
|character/                         |
|   │── README.md                   |
|   │── character-id-1.graphql      |
|   │── character-id-1-output.json  |
|   │── character-id-2.graphql      |
|   │── character-id-2-output.json  |
|   │── character-id-3.graphql      |
|   │── character-id-3-output.json  |
|   │── character-id-4.graphql      |
|   │── character-id-4-output.json  |
🔍 Instructions
Use the provided GraphQL endpoint.

Write a query using:

graphql
Copy
Edit
character(id: ID!)
Replace ID! with 1, 2, 3, and 4 in separate queries.

Each query must fetch:

id

name

status

species

type

gender

Save each query in its respective .graphql file.

Save the results of each query in a .json file with the same ID reference.

🛠 Example Query
graphql
Copy
Edit
{
  character(id: 1) {
    id
    name
    status
    species
    type
    gender
  }
}
✅ Expected Output (Sample)
json
Copy
Edit
{
  "data": {
    "character": {
      "id": "1",
      "name": "Rick Sanchez",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Male"
    }
  }
}
📜 Files to Submit
character-id-1.graphql

character-id-1-output.json

character-id-2.graphql

character-id-2-output.json

character-id-3.graphql

character-id-3-output.json

character-id-4.graphql

character-id-4-output.json

🏷 Repository
GitHub repository: alx-graphql-0x00

Directory: character