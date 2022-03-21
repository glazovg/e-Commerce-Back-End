# e-Commerce Back-End
## Description
This is a back-end project to handle some funtionalities for an e-Commerce, this project can be complemented by adding more functionality like adding routes and models for users, payment methods, etcetera.
    
## Table of Contents
        
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [How to Contribute](#how-to-contribute)
- [Tests](#tests)
- [Questions](#questions)

<a name="installation"></a>
## Installation
1. Run `npm install`to install all the necessary packages.
2. Go to db folder by typing `cd db` and create the schema by:
- Logining to mysql by typing in terminal `mysql -u <your_username> -p`
- Once password is entered mysql prompt is displayed
- Type `source schema.sql;` and hit Enter.
- Once schema y created, type `exit` to exit mysql prompt
3. Go back to root folder `cd ..` and seed the data base by typing `node seeds/index.js` and hit Enter.

<a name="usage"></a>
## Usage
To start using the application we need to use Insomnia to make calls to the created routes. 
1. Start the application with `npm start`
2. Use Insomnia to make any call either by sending GET, POST, PUT or DEL.

Routes that can be reached with Insomnia:

GET `api/products`

GET `api/tags`

GET `api/categories`

GET `api/products/:id`

GET `api/tags/:id`

GET `api/categories/:id`

POST/PUT `api/products`
- Body example:

`{
"product_name": "Basketball",
"price": 200.00,
"stock": 3,
"tagIds": [1, 2, 3, 4]
}`

POST/PUT `api/tags`
- Body example:

`{
	"tag_name": "technology"
}`

POST/PUT `api/categories`
- Body example:

`{
	"category_name": "gaming"
}`

DELETE `api/products/:id`

DELETE `api/tags/:id`

DELETE `api/categories/:id`

*NOTE: For POST, PUT and DELETE methods when response returns 1 the request was applied successfully and when retunrs 0 there was a problem with the request.*
    
<a name="license"></a>
## License
Licensed under the ISC License (ISC).
    
---    
<a name="how-to-contribute"></a>
## How to Contribute
Please follow the steps:
1. Clone the repository in https://github.com/glazovg/e-Commerce-Back-End
2. Go to the project's folder and run `npm install`
3. Create a local branch and you will be all set.

<a name="tests"></a>
## Tests
This repository does not have tests yet, but once added it will be `npm run test`

<a name="questions"></a>
## Questions
If you have any questions or concerns, please contact me:

- By github profile https://github.com/glazovg
- By email glazovg@gmail.com, please with a brief description in the Subject (Bug, Suggestions, Question, Doubts).
