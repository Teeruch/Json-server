#Readme JSON-SERVER

https://github.com/typicode/json-server

npm intall -g json-server

create db.js

json-server --watch db.json

#FakeAPI
npm install faker

create new javascript file
##########################

https://pastebin.com/taZqrsNn

module.exports = () => {
  var faker = require('faker');
  const data = { products: [] }
  for (let i = 0; i < 10; i++) {
    data.products.push({
        productCode: faker.commerce.product(),
        productName: faker.commerce.productName(),
        price: faker.commerce.price(),
        rating: faker.random.number({min: 1, max: 5})  })
  }
  return data
}

and save file **example generate.js
##########################

json-server generate.js