writeCode

Write code to:-
var players = [
  {
    name: 'user 1',
    age: 26,
    email: 'user1@gmail.com',
    bid_price: 200,
  },
  {
    name: 'user 2',
    age: 26,
    email: 'user2@gmail.com',
    bid_price: 200,
  },
  {
    name: 'user 3',
    age: 26,
    email: 'user3@gmail.com',
    bid_price: 200,
  },
  {
    name: 'user 4',
    age: 26,
    email: 'user4@gmail.com',
    bid_price: 200,
  },
];

- create a database named `sports`.
use sports;
- list all databases present in local mongod server.
show dbs;
- create 3 collections named `cricket`, `football`, `TT` in sports databse.
db.createCollection("cricket");
db.createCollection("football");
db.createCollection("TT");

- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
db.cricket.insertMany(players);
db.football.insertMany(players);
db.TT.insertMany(players);

- list all collections in sports database.
 show collections;

- rename `TT` collection to `tennis`.
db.TT.renameCollection("tennis");

- create a capped collection called `khokho` which should have max 3 documents.
db.createCollection('khokho',{capped: true, size: 2048, max: 3});

  Try inserting more than 3 and see what happens?
  If we are try to add more then 3 documents it will ommit the previous one`

- check whether a collection is capped or not?
db.khokho.isCapped();
- drop all documents from `football` collection.
db.football.remove({});
- delete cricket collection completely.
 db.cricket.drop()
- delete sports database.
db.sports.drop()/db.dropDatabase();

- check which database you are connected to ?
show dbs
- connect to test database
use test
/*********************/

