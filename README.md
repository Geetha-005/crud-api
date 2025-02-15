first create a folder :mkdir folder_name
 cd folder_name
 npm init -y
 npm install express mongoose nodemon

the folder structure:
folder_name:
 -->node_modules
 -->models
     -->product.model.js
 -->index.js


 the above is the folder structure: index.js is the entry point 

to connect the mongodb atlas
 const MONGO_URL=mongodb+srv://myUser:myPassword@cluster0.mongodb.net/myDatabase?retryWrites=true&w=majority
 user_name and password can mkdify with the our data


 after completing the above steps :
 run the code with :node index.js(starting point)
 or otherwise:
    modify the package.json:
     "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "serve": "node index.js",
    "dev": "nodemon index.js"
  },

  for the above change we can run the code with: npm run dev



after test the crud operations in postan rest api:
CRUD MEANS CREATE,READ,UPDATE AND DELETE

CREATE----POST
READ----GET
UPDATE---PUT
DELETE---DELETE



GET---->  localhost:5000/api/products
  to get the all products in the databse

  localhost:5000/api/product/:id
   to get the item in the databse based on id 



POST---->localhost:5000/api/products
to send the json data to database

{
name:string 
quantity:number
price:number
image:string
}

{
    "name":"Ac",
    "quantity":1,
    "price":100000,
    "iamge":"https://th.bing.com/th/id/OIP._efNH1rK-rcc5XNeK1pAfAHaHa?w=187&h=187&c=7&r=0&o=5&pid=1.7"

}

POST---localhost:5000/api/product/:id 

based on id we can modify the existing data 


DELETE----localhost:localhost:5000/api/product/:id 

based on id we can delete OR remove that particular item in the database.



HAPPY CODING!!!






















 
